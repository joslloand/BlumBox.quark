# BlumBox.quark

The Blumlein Box (aka BlumBox) is a collection of stereo imaging transforms and analyses 
packaged together as a SuperCollider Quark. 

## Credits
Developed by Emmett Miller with the guidance of Dr. Joseph Anderson, whose paper Classical Stereo Imaging Transforms--A Review serves as the basis for this project, and [DXARTS](https://dxarts.washington.edu/) at the [University of Washington](https://uw.edu/).

## Installing

### Requirements
BlumBox.quark was developed on SuperCollider 3.12.2. Though previous versions may be compatible, it might not be a bad idea to install the latest SuperCollider update.

To install the quark, run the following in SuperCollider:
```supercollider
Quarks.install("https://github.com/emillwe/BlumBox.quark.git");
```

If you've already installed BlumBox, you can make sure all dependencies are up to date using the QuarksGui:
```supercollider
Quarks.gui
```

## The Transforms
The Blumlein Box implements the following 9 stereo transforms:

### MS to LR
Transforms a signal from the MS domain to the LR domain

### LR to MS
Transforms a signal from the LR domain to the MS domain

### Rotation
Rotates a stereo signal, preserving relative positions in the stereo field

### Width
Widens or narrows a stereo signal

### Balance
Stereo panning as implemented on most consumer electronics--compresses a stereo signal towards the L or R axis

### Middle Panorama
Rotates the M-axis of a stereo image, leaving the S-axis in place

### Asymmetry
Rotates the S-axis of a stereo image, leaving the M-axis in place

### Left Panorama
Rotates only the L-axis of a stereo image

### Right Panorama
Rotates only the R-axis of a stereo image

## The Analyses
The Blumlein Box also includes the following 5 stereo imaging analysis functions. Each has the option to return either an instantaneous or time-average value.

### Power
Returns the power of a stereo signal

### Balance
Distribution of power along the L-R axis. 

### Correlation
Degree of similarity between left and right channels, i.e. the distribution of power along the M-S axis

### Angle
Apparent source direction in radians of a stereo image

### Radius
Encoding radius of a stereo image

## References
1. Anderson, J. L., "Classic Stereo Imaging Transforms: A Review", published in Spanish in Basso, G., Di Liscia, O. P. & Pampin, J. (editors)(2009). "Música y espacio: ciencia, tecnología y estética". Buenos Aires, Universidad Nacional de Quilmes.

2. Streicher, Ron., and F. Alton Everest. The New Stereo Soundbook. Audio Engineering Associates, 2006.

3. American reprint: Blumlein, A. D. (1958). "British Patent Specification 394,325 'Improvements in and relating to Sound-transmission, Sound-recording and Sound-reproducing Systems'" (PDF). Journal of the Audio Engineering Society. 6 (2): 32–40.
