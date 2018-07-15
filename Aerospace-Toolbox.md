Maps functionality from the MATLAB [Aerospace Toolbox](https://www.mathworks.com/help/aerotbx/index.html) to equivalent(s) in Julia.

Related Julia packages:
* [ReferenceFrameRotations.jl](https://github.com/JuliaSpace/ReferenceFrameRotations.jl)

# Data Import
* [[datcomimport]] Bring DATCOM file into MATLAB environment

# Coordinate Systems

## Axes Transformations
* [[angle2dcm]] Convert rotation angles to direction cosine matrix
* [[angle2quat]] Convert rotation angles to quaternion
* [[angle2rod]] Convert rotation angles to Euler-Rodrigues vector
* [[dcm2angle]] Create rotation angles from direction cosine matrix
* [[rod2angle]] Convert Euler-Rodrigues vector to rotation angles
* [[quat2angle]] Convert quaternion to rotation angles
* [[dcm2alphabeta]] Convert direction cosine matrix to angle of attack and sideslip angle
* [[dcm2latlon]] Convert direction cosine matrix to geodetic latitude and longitude
* [[dcm2quat]] Convert direction cosine matrix to quaternion
* [[dcm2rod]] Convert direction cosine matrix to Euler-Rodrigues vector
* [[dcmbody2wind]] Convert angle of attack and sideslip angle to direction cosine matrix
* [[dcmecef2ned]] Convert geodetic latitude and longitude to direction cosine matrix
* [[dcmeci2ecef]] Convert Earth-centered inertial (ECI) to Earth-centered Earth-fixed (ECEF) coordinates
* [[quat2dcm]] Convert quaternion to direction cosine matrix
* [[rod2dcm]] Convert Euler-Rodrigues vector to direction cosine matrix
* [[ecef2lla]] Convert Earth-centered Earth-fixed (ECEF) coordinates to geodetic coordinates
* [[eci2lla]] Convert Earth-centered inertial (ECI) coordinates to latitude, longitude, altitude (LLA) geodetic coordinates
* [[flat2lla]] Convert from flat Earth position to array of geodetic latitude, longitude, and altitude coordinates
* [[lla2ecef]] Convert geodetic coordinates to Earth-centered Earth-fixed (ECEF) coordinates
* [[lla2eci]] Convert geodetic latitude, longitude, altitude (LLA) coordinates to Earth-centered inertial (ECI) coordinates
* [[lla2flat]] Convert from geodetic latitude, longitude, and altitude to flat Earth position
* [[geoc2geod]] Convert geocentric latitude to geodetic latitude
* [[geod2geoc]] Convert geodetic latitude to geocentric latitude
* [[angle2quat]] Convert rotation angles to quaternion
* [[dcm2quat]] Convert direction cosine matrix to quaternion
* [[quat2angle]] Convert quaternion to rotation angles
* [[quat2dcm]] Convert quaternion to direction cosine matrix
* [[quat2rod]] Convert quaternion to Euler-Rodrigues vector
* [[rod2quat]] Convert Euler-Rodrigues vector to quaternion
* [[eci2aer]] Convert Earth-centered inertial (ECI) coordinates to azimuth, elevation, slant range (AER) coordinates
* [[angle2rod]] Convert rotation angles to Euler-Rodrigues vector
* [[dcm2rod]] Convert direction cosine matrix to Euler-Rodrigues vector
* [[quat2rod]] Convert quaternion to Euler-Rodrigues vector
* [[rod2angle]] Convert Euler-Rodrigues vector to rotation angles
* [[rod2dcm]] Convert Euler-Rodrigues vector to direction cosine matrix
* [[rod2quat]] Convert Euler-Rodrigues vector to quaternion

## Flight Parameters and Quaternion Math
* [[airspeed]] Airspeed from velocity
* [[alphabeta]] Incidence and sideslip angles
* [[correctairspeed]] Convert from one of other two airspeeds to equivalent airspeed (EAS), calibrated airspeed (CAS), or true airspeed (TAS)
* [[dpressure]] Compute dynamic pressure using velocity and density
* [[machnumber]] Compute Mach number using velocity and speed of sound
* [[rrdelta]] Compute relative pressure ratio
* [[rrsigma]] Compute relative density ratio
* [[rrtheta]] Compute relative temperature ratio
* [[quatconj]] Calculate conjugate of quaternion
* [[quatdivide]] Divide quaternion by another quaternion
* [[quatexp]] Exponential of quaternion
* [[quatinterp]] Quaternion interpolation between two quaternions
* [[quatinv]] Calculate inverse of quaternion
* [[quatlog]] Natural logarithm of quaternion
* [[quatmod]] Calculate modulus of quaternion
* [[quatmultiply]] Calculate product of two quaternions
* [[quatnorm]] Calculate norm of quaternion
* [[quatnormalize]] Normalize quaternion
* [[quatpower]] Power of quaternion
* [[quatrotate]] Rotate vector by quaternion

# Unit Conversions
* [[aeroReadIERSData]] File containing current International Astronomical Union (IAU) 2000A Earth orientation data
* [[convacc]] Convert from acceleration units to desired acceleration units
* [[convang]] Convert from angle units to desired angle units
* [[convangacc]] Convert from angular acceleration units to desired angular acceleration units
* [[convangvel]] Convert from angular velocity units to desired angular velocity units
* [[convdensity]] Convert from density units to desired density units
* [[convforce]] Convert from force units to desired force units
* [[convlength]] Convert from length units to desired length units
* [[convmass]] Convert from mass units to desired mass units
* [[convpres]] Convert from pressure units to desired pressure units
* [[convtemp]] Convert from temperature units to desired temperature units
* [[convvel]] Convert from velocity units to desired velocity units
* [[deltaUT1]] Calculate difference between Coordinated Universal Time (UTC) and Principal Universal Time (UT1)
* [[decyear]] Decimal year calculator
* [[juliandate]] Julian date calculator
* [[leapyear]] Determine leap year
* [[mjuliandate]] Modified Julian date calculator
* [[tdbjuliandate]] terrConvert from Barycentric Dynamical Time Estimate to Julian date

# Environment
* [[aeroDataPackage]] Start Add-On Explorer to download, install, or uninstall aerospace-specific data
* [[atmoscira]] Use COSPAR International Reference Atmosphere 1986 model
* [[atmoscoesa]] Use 1976 COESA model
* [[atmoshwm]] Implement horizontal wind model
* [[atmosisa]] Use International Standard Atmosphere model
* [[atmoslapse]] Use Lapse Rate Atmosphere model
* [[atmosnonstd]] Use climatic data from MIL-STD-210 or MIL-HDBK-310
* [[atmosnrlmsise00]] Implement mathematical representation of 2001 United States Naval Research Laboratory Mass Spectrometer and Incoherent Scatter Radar Exosphere
* [[atmospalt]] Calculate pressure altitude based on ambient pressure
* [[earthNutation]] Implement Earth nutation
* [[moonLibration]] Moon librations
* [[planetEphemeris]] Position and velocity of astronomical objects
* [[geocradius]] Convert from geocentric latitude to radius of ellipsoid planet
* [[geoidegm96]] Calculate geoid height as determined from EGM96 Geopotential Model
* [[geoidheight]] Calculate geoid height
* [[gravitycentrifugal]] Implement centrifugal effect of planetary gravity
* [[gravitysphericalharmonic]] Implement spherical harmonic representation of planetary gravity
* [[gravitywgs84]] Implement 1984 World Geodetic System (WGS84) representation of Earth's gravity
* [[gravityzonal]] Implement zonal harmonic representation of planetary gravity
* [[igrfmagm]] Calculate Earth magnetic field and secular variation using International Geomagnetic Reference Field
* [[wrldmagm]] Use World Magnetic Model

# Gas Dynamics
* [[flowfanno]] Fanno line flow relations
* [[flowisentropic]] Isentropic flow ratios
* [[flownormalshock]] Normal shock relations
* [[flowprandtlmeyer]] Calculate Prandtl-Meyer functions for expansion waves
* [[flowrayleigh]] Rayleigh line flow relations

# Visualize Trajectory and Attitude

## Axes Transformations
* [[angle2dcm]] Convert rotation angles to direction cosine matrix
* [[angle2quat]] Convert rotation angles to quaternion
* [[angle2rod]] Convert rotation angles to Euler-Rodrigues vector
* [[dcm2angle]] Create rotation angles from direction cosine matrix
* [[rod2angle]] Convert Euler-Rodrigues vector to rotation angles
* [[quat2angle]] Convert quaternion to rotation angles
* [[angle2dcm]] Convert rotation angles to direction cosine matrix
* [[dcm2alphabeta]] Convert direction cosine matrix to angle of attack and sideslip angle
* [[dcm2latlon]] Convert direction cosine matrix to geodetic latitude and longitude
* [[dcm2quat]] Convert direction cosine matrix to quaternion
* [[dcm2rod]] Convert direction cosine matrix to Euler-Rodrigues vector
* [[dcmbody2wind]] Convert angle of attack and sideslip angle to direction cosine matrix
* [[dcmecef2ned]] Convert geodetic latitude and longitude to direction cosine matrix
* [[dcmeci2ecef]] Convert Earth-centered inertial (ECI) to Earth-centered Earth-fixed (ECEF) coordinates
* [[quat2dcm]] Convert quaternion to direction cosine matrix
* [[rod2dcm]] Convert Euler-Rodrigues vector to direction cosine matrix
* [[ecef2lla]] Convert Earth-centered Earth-fixed (ECEF) coordinates to geodetic coordinates
* [[eci2lla]] Convert Earth-centered inertial (ECI) coordinates to latitude, longitude, altitude (LLA) geodetic coordinates
* [[flat2lla]] Convert from flat Earth position to array of geodetic latitude, longitude, and altitude coordinates
* [[lla2ecef]] Convert geodetic coordinates to Earth-centered Earth-fixed (ECEF) coordinates
* [[lla2eci]] Convert geodetic latitude, longitude, altitude (LLA) coordinates to Earth-centered inertial (ECI) coordinates
* [[lla2flat]] Convert from geodetic latitude, longitude, and altitude to flat Earth position
* [[geoc2geod]] Convert geocentric latitude to geodetic latitude
* [[geod2geoc]] Convert geodetic latitude to geocentric latitude
* [[angle2quat]] Convert rotation angles to quaternion
* [[dcm2quat]] Convert direction cosine matrix to quaternion
* [[quat2angle]] Convert quaternion to rotation angles
* [[quat2dcm]] Convert quaternion to direction cosine matrix
* [[quat2rod]] Convert quaternion to Euler-Rodrigues vector
* [[rod2quat]] Convert Euler-Rodrigues vector to quaternion
* [[eci2aer]] Convert Earth-centered inertial (ECI) coordinates to azimuth, elevation, slant range (AER) coordinates
* [[angle2rod]] Convert rotation angles to Euler-Rodrigues vector
* [[dcm2rod]] Convert direction cosine matrix to Euler-Rodrigues vector
* [[quat2rod]] Convert quaternion to Euler-Rodrigues vector
* [[rod2angle]] Convert Euler-Rodrigues vector to rotation angles
* [[rod2dcm]] Convert Euler-Rodrigues vector to direction cosine matrix
* [[rod2quat]] Convert Euler-Rodrigues vector to quaternion

## Flight Simulator Interfaces
* [[Aero]].FlightGearAnimation Construct FlightGear animation object

## MATLAB Based Animation
* [[Aero]].Animation Visualize aerospace animation
* [[Aero]].Body Create body object for use with animation object
* [[Aero]].Camera Construct camera object for use with animation object
* [[Aero]].Geometry Construct 3-D geometry for use with animation object

## Virtual Reality Animation
* [[Aero]].Node Create node object for use with virtual reality animation
* [[Aero]].Viewpoint Create viewpoint object for use in virtual reality animation
* [[Aero]].VirtualRealityAnimation Construct virtual reality animation object
