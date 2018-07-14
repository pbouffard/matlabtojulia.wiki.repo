Maps functionality from the MATLAB [Control System Toolbox](https://www.mathworks.com/help/control/index.html) to equivalent(s) in Julia.

Related Julia packages:
* [ControlSystems.jl](https://github.com/JuliaControl/ControlSystems.jl)

***

# Dynamic System Models

## Linear System Representation

## Basic Models
* [[tf]]	Create transfer function model, convert to transfer function model
* [[zpk]]	Create zero-pole-gain model; convert to zero-pole-gain model
* [[ss]]	Create state-space model, convert to state-space model
* [[frd]]	Create frequency-response data model, convert to frequency-response data model
* [[filt]]	Specify discrete transfer functions in DSP format
* [[dss]]	Create descriptor state-space models
* [[pid]]	Create PID controller in parallel form, convert to parallel-form PID controller
* [[pidstd]]	Create a PID controller in standard form, convert to standard-form PID controller
* [[pid2]]	Create 2-DOF PID controller in parallel form, convert to parallel-form 2-DOF PID controller
* [[pidstd2]]	Create 2-DOF PID controller in standard form, convert to standard-form 2-DOF PID controller
* [[rss]]	Generate random continuous test model
* [[drss]]	Generate random discrete test model

## Tunable Models
* [[tunableGain]]	Tunable static gain block
* [[tunablePID]]	Tunable PID controller
* [[tunablePID2]]	Tunable two-degree-of-freedom PID controller
* [[tunableSS]]	Tunable fixed-order state-space model
* [[tunableTF]]	Tunable transfer function with fixed number of poles and zeros
* [[realp]]	Real tunable parameter
* [[AnalysisPoint]]	Points of interest for linear analysis
* [[genss]]	Generalized state-space model
* [[genfrd]]	Generalized frequency response data (FRD) model
* [[genmat]]	Generalized matrix with tunable parameters
* [[getLoopTransfer]]	Open-loop transfer function of control system
* [[getIOTransfer]]	Closed-loop transfer function from generalized model of control system
* [[getSensitivity]]	Sensitivity function from generalized model of control system
* [[getCompSensitivity]]	Complementary sensitivity function from generalized model of control system
* [[getPoints]]	Get list of analysis points in generalized model of control system
* [[replaceBlock]]	Replace or update Control Design Blocks in Generalized LTI model
* [[sampleBlock]]	Sample Control Design blocks in generalized model
* [[rsampleBlock]]	Randomly sample Control Design blocks in generalized model
* [[getValue]]	Current value of Generalized Model
* [[setValue]]	Modify current value of Control Design Block
* [[getBlockValue]]	Current value of Control Design Block in Generalized Model
* [[setBlockValue]]	Modify value of Control Design Block in Generalized Model
* [[showBlockValue]]	Display current value of Control Design Blocks in Generalized Model
* [[showTunable]]	Display current value of tunable Control Design Blocks in Generalized Model
* [[nblocks]]	Number of blocks in Generalized matrix or Generalized LTI model
* [[getLFTModel]]	Decompose generalized LTI model

## Models with Time Delays
* [[pade]]	Padé approximation of model with time delays
* [[absorbDelay]]	Replace time delays by poles at z = 0 or phase shift
* [[thiran]]	Generate fractional delay filter based on Thiran approximation
* [[hasdelay]]	True for linear model with time delays
* [[hasInternalDelay]]	Determine if model has internal delays
* [[totaldelay]]	Total combined I/O delays for LTI model
* [[delayss]]	Create state-space models with delayed inputs, outputs, and states
* [[setDelayModel]]	Construct state-space model with internal delays
* [[getDelayModel]]	State-space representation of internal delays

## Model Attributes
* [[get]]	Access model property values
* [[set]]	Set or modify model properties
* [[tfdata]]	Access transfer function data
* [[zpkdata]]	Access zero-pole-gain data
* [[ssdata]]	Access state-space model data
* [[frdata]]	Access data for frequency response data (FRD) object
* [[piddata]]	Access coefficients of parallel-form PID controller
* [[pidstddata]]	Access coefficients of standard-form PID controller
* [[piddata2]]	Access coefficients of parallel-form 2-DOF PID controller
* [[pidstddata2]]	Access coefficients of standard-form 2-DOF PID controller
* [[dssdata]]	Extract descriptor state-space data
* [[chgFreqUnit]]	Change frequency units of frequency-response data model
* [[chgTimeUnit]]	Change time units of dynamic system
* [[isct]]	Determine if dynamic system model is in continuous time
* [[isdt]]	Determine if dynamic system model is in discrete time
* [[isempty]]	Determine whether dynamic system model is empty
* [[isfinite]]	Determine if model has finite coefficients
* [[isParametric]]	Determine if model has tunable parameters
* [[isproper]]	Determine if dynamic system model is proper
* [[isreal]]	Determine if model has real-valued coefficients
* [[issiso]]	Determine if dynamic system model is single-input/single-output (SISO)
* [[isstable]]	Determine whether system is stable
* [[isstatic]]	Determine if model is static or dynamic
* [[order]]	Query model order
* [[ndims]]	Query number of dimensions of dynamic system model or model array
* [[size]]	Query output/input/array dimensions of input–output model and number of frequencies of FRD model

### Model Arrays
* [[stack]]	Build model array by stacking models or model arrays along array dimensions
* [[nmodels]]	Number of models in model array
* [[permute]]	Rearrange array dimensions in model arrays
* [[reshape]]	Change shape of model array
* [[repsys]]	Replicate and tile models
* [[voidModel]]	Mark missing or irrelevant models in model array
* [[sampleBlock]]	Sample Control Design blocks in generalized model
* [[rsampleBlock]]	Randomly sample Control Design blocks in generalized model

## Model Interconnection
* [[feedback]]	Feedback connection of two models
* [[connect]]	Block diagram interconnections of dynamic systems
* [[sumblk]]	Summing junction for name-based interconnections
* [[series]]	Series connection of two models
* [[parallel]]	Parallel connection of two models
* [[append]]	Group models by appending their inputs and outputs
* [[blkdiag]]	Block-diagonal concatenation of models
* [[imp2exp]]	Convert implicit linear relationship to explicit input-output relation
* [[inv]]	Invert models
* [[lft]]	Generalized feedback interconnection of two models (Redheffer star product)
* [[connectOptions]]	Options for the connect command

## Model Transformation

### Model Type Conversion
* [[tf]]	Create transfer function model, convert to transfer function model
* [[zpk]]	Create zero-pole-gain model; convert to zero-pole-gain model
* [[ss]]	Create state-space model, convert to state-space model
* [[frd]]	Create frequency-response data model, convert to frequency-response data model
* [[pid]]	Create PID controller in parallel form, convert to parallel-form PID controller
* [[pidstd]]	Create a PID controller in standard form, convert to standard-form PID controller
* [[pid2]]	Create 2-DOF PID controller in parallel form, convert to parallel-form 2-DOF PID controller
* [[pidstd2]]	Create 2-DOF PID controller in standard form, convert to standard-form 2-DOF PID controller
* [[make1DOF]]	Convert 2-DOF PID controller to 1-DOF controller
* [[make2DOF]]	Convert 1-DOF PID controller to 2-DOF controller
* [[getComponents]]	Extract SISO control components from a 2-DOF PID controller

### Continuous-Discrete Conversion
* [[c2d]]	Convert model from continuous to discrete time
* [[d2c]]	Convert model from discrete to continuous time
* [[d2d]]	Resample discrete-time model
* [[upsample]]	Upsample discrete-time models
* [[c2dOptions]]	Create option set for continuous- to discrete-time conversions
* [[d2cOptions]]	Create option set for discrete- to continuous-time conversions
* [[d2dOptions]]	Create option set for discrete-time resampling

### State-Coordinate Transformation
* [[balreal]]	Gramian-based input/output balancing of state-space realizations
* [[canon]]	State-space canonical realization
* [[prescale]]	Optimal scaling of state-space models
* [[ss2ss]]	State coordinate transformation for state-space model
* [[xperm]]	Reorder states in state-space models

### Modal Decomposition
* [[modsep]]	Region-based modal decomposition
* [[stabsep]]	Stable-unstable decomposition
* [[stabsepOptions]]	Options for stable-unstable decomposition
* [[freqsep]]	Slow-fast decomposition
* [[freqsepOptions]]	Options for slow-fast decomposition
* [[spectralfact]]	Spectral factorization of linear systems

### Model Reduction
* [[balred]]	Model order reduction
* [[balredOptions]]	Create option set for model order reduction
* [[balreal]]	Gramian-based input/output balancing of state-space realizations
* [[minreal]]	Minimal realization or pole-zero cancelation
* [[sminreal]]	Structural pole/zero cancellations
* [[modred]]	Eliminate states from state-space models
* [[freqsep]]	Slow-fast decomposition
* [[freqsepOptions]]	Options for slow-fast decomposition
* [[hsvd]]	Hankel singular values of dynamic system
* [[hsvplot]]	Plot Hankel singular values and return plot handle
* [[hsvdOptions]]	Create option set for computing Hankel singular values and input/output balancing

## Linear Analysis

### Time and Frequency Domain Analysis
* [[step]]	Step response plot of dynamic system; step response data
* [[stepinfo]]	Rise time, settling time, and other step-response characteristics
* [[impulse]]	Impulse response plot of dynamic system; impulse response data
* [[initial]]	Initial condition response of state-space model
* [[lsim]]	Simulate time response of dynamic system to arbitrary inputs
* [[lsiminfo]]	Compute linear response characteristics
* [[gensig]]	Generate test input signals for lsim
* [[covar]]	Output and state covariance of system driven by white noise
* [[stepDataOptions]]	Options set for step
* [[bode]]	Bode plot of frequency response, or magnitude and phase data
* [[bodemag]]	Bode magnitude response of LTI models
* [[nyquist]]	Nyquist plot of frequency response
* [[nichols]]	Nichols chart of frequency response
* [[ngrid]]	Superimpose Nichols chart on Nichols plot
* [[sigma]]	Singular values plot of dynamic system
* [[freqresp]]	Frequency response over grid
* [[evalfr]]	Evaluate frequency response at given frequency
* [[dcgain]]	Low-frequency (DC) gain of LTI system
* [[bandwidth]]	Frequency response bandwidth
* [[getPeakGain]]	Peak gain of dynamic system frequency response
* [[getGainCrossover]]	Crossover frequencies for specified gain
* [[fnorm]]	Pointwise peak gain of FRD model
* [[norm]]	Norm of linear model
* [[db2mag]]	Convert decibels (dB) to magnitude
* [[mag2db]]	Convert magnitude to decibels (dB)

### Stability Analysis
* [[pole]]	Compute poles of dynamic system
* [[zero]]	Zeros and gain of SISO dynamic system
* [[damp]]	Natural frequency and damping ratio
* [[dsort]]	Sort discrete-time poles by magnitude
* [[esort]]	Sort continuous-time poles by real part
* [[tzero]]	Invariant zeros of linear system
* [[pzplot]]	Pole-zero map of dynamic system model with plot customization options
* [[iopzplot]]	Plot pole-zero map for I/O pairs and return plot handle
* [[allmargin]]	Gain margin, phase margin, delay margin and crossover frequencies
* [[margin]]	Gain margin, phase margin, and crossover frequencies

### Sensitivity Analysis
* [[sampleBlock]]	Sample Control Design blocks in generalized model
* [[rsampleBlock]]	Randomly sample Control Design blocks in generalized model

### Passivity and Sector Bounds
* [[isPassive]]	Check passivity of linear systems
* [[getPassiveIndex]]	Compute passivity index of linear system
* [[passiveplot]]	Compute or plot passivity index as function of frequency
* [[getSectorIndex]]	Compute conic-sector index of linear system
* [[getSectorCrossover]]	Crossover frequencies for sector bound
* [[sectorplot]]	Compute or plot sector index as function of frequency

### Plot Customization
* [[impulseplot]]	Plot impulse response and return plot handle
* [[initialplot]]	Plot initial condition response and return plot handle
* [[lsimplot]]	Simulate response of dynamic system to arbitrary inputs and return plot handle
* [[stepplot]]	Plot step response and return plot handle
* [[bodeplot]]	Plot Bode frequency response with additional plot customization options
* [[nicholsplot]]	Plot Nichols frequency responses and return plot handle
* [[nyquistplot]]	Nyquist plot with additional plot customization options
* [[sigmaplot]]	Plot singular values of frequency response and return plot handle
* [[bodeoptions]]	Create list of Bode plot options
* [[hsvoptions]]	Plot options for hsvplot
* [[nicholsoptions]]	Create list of Nichols plot options
* [[nyquistoptions]]	List of Nyquist plot options
* [[pzoptions]]	Create list of pole/zero plot options
* [[sigmaoptions]]	Create list of singular-value plot options
* [[timeoptions]]	Create list of time plot options
* [[setoptions]]	Set plot options for response plot
* [[getoptions]]	Return @PlotOptions handle or plot options property
* [[ctrlpref]]	Set Control System Toolbox preferences
* [[updateSystem]]	Update dynamic system data in a response plot

# Control System Design and Tuning

## PID Controller Tuning
* [[pidTuner]]	Open PID Tuner for PID tuning
* [[pidtune]]	PID tuning algorithm for linear plant model
* [[pidtuneOptions]]	Define options for pidtune command

## Classical Control Design
* [[rlocus]]	Root locus plot of dynamic system
* [[rlocusplot]]	Plot root locus and return plot handle
* [[sisoinit]]	Configure Control System Designer at startup

## State-Space Control Design and Estimation

### State-Space Control Design
* [[lqr]]	Linear-Quadratic Regulator (LQR) design
* [[lqry]]	Form linear-quadratic (LQ) state-feedback regulator with output weighting
* [[lqi]]	Linear-Quadratic-Integral control
* [[dlqr]]	Linear-quadratic (LQ) state-feedback regulator for discrete-time state-space system
* [[lqrd]]	Design discrete linear-quadratic (LQ) regulator for continuous plant
* [[lqg]]	Linear-Quadratic-Gaussian (LQG) design
* [[lqgreg]]	Form linear-quadratic-Gaussian (LQG) regulator
* [[lqgtrack]]	Form Linear-Quadratic-Gaussian (LQG) servo controller
* [[augstate]]	Append state vector to output vector
* [[norm]]	Norm of linear model
* [[estim]]	Form state estimator given estimator gain
* [[place]]	Pole placement design
* [[reg]]	Form regulator given state-feedback and estimator gains

### State Estimation
* [[kalman]]	Kalman filter design, Kalman estimator
* [[kalmd]]	Design discrete Kalman estimator for continuous plant
* [[estim]]	Form state estimator given estimator gain
* [[extendedKalmanFilter]]	Create extended Kalman filter object for online state estimation
* [[unscentedKalmanFilter]]	Create unscented Kalman filter object for online state estimation
* [[particleFilter]]	Particle filter object for online state estimation
* [[correct]]	Correct state and state estimation error covariance using extended or unscented Kalman filter, or particle filter and measurements
* [[predict]]	Predict state and state estimation error covariance at next time step using extended or unscented Kalman filter, or particle filter
* [[initialize]]	Initialize the state of the particle filter
* [[clone]]	Copy online state estimation object

## Multiloop, Multiobjective Tuning

### Programmatic Tuning

#### Setup for Tuning Simulink Models
* [[slTuner]]	Interface for control system tuning of Simulink models
* [[slTunerOptions]]	Set slTuner interface options
* [[addBlock]]	Add block to list of tuned blocks for slTuner interface
* [[addOpening]]	Add signal to list of openings for slLinearizer or slTuner interface
* [[addPoint]]	Add signal to list of analysis points for slLinearizer or slTuner interface
* [[refresh]]	Resynchronize slLinearizer or slTuner interface with current model state
* [[removeAllOpenings]]	Remove all openings from list of permanent openings in slLinearizer or slTuner interface
* [[removeAllPoints]]	Remove all points from list of analysis points in slLinearizer or slTuner interface
* [[removeBlock]]	Remove block from list of tuned blocks in slTuner interface
* [[removeOpening]]	Remove opening from list of permanent loop openings in slLinearizer or slTuner interface
* [[removePoint]]	Remove point from list of analysis points in slLinearizer or slTuner interface
* [[setBlockParam]]	Set parameterization of tuned block in slTuner interface
* [[setBlockRateConversion]]	Set rate conversion settings for tuned block in slTuner interface
* [[setBlockValue]]	Set value of tuned block parameterization in slTuner interface
* [[writeBlockValue]]	Update block values in Simulink model
* [[writeLookupTableData]]	Update portion of tuned lookup table
* [[getBlockParam]]	Get parameterization of tuned block in slTuner interface
* [[getBlockRateConversion]]	Get rate conversion settings for tuned block in slTuner interface
* [[getBlockValue]]	Get current value of tuned block parameterization in slTuner interface
* [[getOpenings]]	Get list of openings for slLinearizer or slTuner interface
* [[getPoints]]	Get list of analysis points for slLinearizer or slTuner interface
* [[showTunable]]	Show value of parameterizations of tunable blocks of slTuner interface

#### Setup for Tuning MATLAB Models
* [[tf]]	Create transfer function model, convert to transfer function model
* [[zpk]]	Create zero-pole-gain model; convert to zero-pole-gain model
* [[ss]]	Create state-space model, convert to state-space model
* [[tunableGain]]	Tunable static gain block
* [[tunableTF]]	Tunable transfer function with fixed number of poles and zeros
* [[tunablePID]]	Tunable PID controller
* [[tunablePID2]]	Tunable two-degree-of-freedom PID controller
* [[tunableSS]]	Tunable fixed-order state-space model
* [[realp]]	Real tunable parameter
* [[AnalysisPoint]]	Points of interest for linear analysis
* [[connect]]	Block diagram interconnections of dynamic systems
* [[feedback]]	Feedback connection of two models

#### Tuning Goals
* [[TuningGoal]].StepTracking	Step response requirement for control system tuning
* [[TuningGoal]].StepRejection	Step disturbance rejection requirement for control system tuning
* [[TuningGoal]].Transient	Transient matching requirement for control system tuning
* [[TuningGoal]].LQG	Linear-Quadratic-Gaussian (LQG) goal for control system tuning
* [[TuningGoal]].Gain	Gain constraint for control system tuning
* [[TuningGoal]].Variance	Noise amplification constraint for control system tuning
* [[TuningGoal]].Tracking	Tracking requirement for control system tuning
* [[TuningGoal]].Overshoot	Overshoot constraint for control system tuning
* [[TuningGoal]].Rejection	Disturbance rejection requirement for control system tuning
* [[TuningGoal]].Sensitivity	Sensitivity requirement for control system tuning
* [[TuningGoal]].WeightedGain	Frequency-weighted gain constraint for control system tuning
* [[TuningGoal]].WeightedVariance	Frequency-weighted H2 norm constraint for control system tuning
* [[TuningGoal]].MinLoopGain	Minimum loop gain constraint for control system tuning
* [[TuningGoal]].MaxLoopGain	Maximum loop gain constraint for control system tuning
* [[TuningGoal]].LoopShape	Target loop shape for control system tuning
* [[TuningGoal]].Margins	Stability margin requirement for control system tuning
* [[TuningGoal]].Passivity	Passivity constraint for control system tuning
* [[TuningGoal]].ConicSector	Sector bound for control system tuning
* [[TuningGoal]].WeightedPassivity	Frequency-weighted passivity constraint
* [[TuningGoal]].Poles	Constraint on control system dynamics
* [[TuningGoal]].ControllerPoles	Constraint on controller dynamics for control system tuning

#### Tuning, Analysis, and Validation
* [[systune]] (slTuner)	Tune control system parameters in Simulink using slTuner interface
* [[systuneOptions]]	Set options for systune
* [[getIOTransfer]] (slTuner)	Transfer function for specified I/O set using slLinearizer or slTuner interface
* [[getLoopTransfer]] (slTuner)	Open-loop transfer function at specified point using slLinearizer or slTuner interface
* [[getSensitivity]] (slTuner)	Sensitivity function at specified point using slLinearizer or slTuner interface
* [[getCompSensitivity]] (slTuner)	Complementary sensitivity function at specified point using slLinearizer or slTuner interface
* [[writeBlockValue]]	Update block values in Simulink model
* [[systune]]	Tune fixed-structure control systems modeled in MATLAB
* [[systuneOptions]]	Set options for systune
* [[getIOTransfer]]	Closed-loop transfer function from generalized model of control system
* [[getLoopTransfer]]	Open-loop transfer function of control system
* [[getSensitivity]]	Sensitivity function from generalized model of control system
* [[getCompSensitivity]]	Complementary sensitivity function from generalized model of control system
* [[viewGoal]]	View tuning goals; validate design against tuning goals
* [[evalGoal]]	Evaluate tuning goals for tuned control system

### Loop-Shaping Design
* [[slTuner]]	Interface for control system tuning of Simulink models
* [[looptune]]	Tune MIMO feedback loops in Simulink using slTuner interface
* [[looptuneOptions]]	Set options for looptune
* [[loopview]]	Graphically analyze results of control system tuning using slTuner interface
* [[looptuneSetup]]	Construct tuning setup for looptune to tuning setup for systune using slTuner interface
* [[looptune]]	Tune fixed-structure feedback loops
* [[looptuneOptions]]	Set options for looptune
* [[loopview]]	Graphically analyze MIMO feedback loops
* [[looptuneSetup]]	Convert tuning setup for looptune to tuning setup for systune
* [[viewGoal]]	View tuning goals; validate design against tuning goals
* [[evalGoal]]	Evaluate tuning goals for tuned control system

## Gain Scheduling
* [[tunableSurface]]	Create tunable gain surface for gain scheduling
* [[polyBasis]]	Polynomial basis functions for tunable gain surface
* [[fourierBasis]]	Fourier basis functions for tunable gain surface
* [[ndBasis]]	Basis functions for tunable gain surface
* [[viewSurf]]	Visualize gain surface as a function of scheduling variables
* [[evalSurf]]	Evaluate gain surfaces at specific design points
* [[getData]]	Get current values of tunable-surface coefficients
* [[setData]]	Set values of tunable-surface coefficients
* [[codegen]]	Generate MATLAB code for tunable gain surfaces
* [[systune]]	Tune fixed-structure control systems modeled in MATLAB
* [[slTuner]]	Interface for control system tuning of Simulink models
* [[systune]] (slTuner)	Tune control system parameters in Simulink using slTuner interface
* [[voidModel]]	Mark missing or irrelevant models in model array
* [[varyingGoal]]	Variable tuning goal for gain-scheduled controllers
* [[getGoal]]	Evaluate variable tuning goal at specified design point

# Matrix Computations
* [[lyap]]	Continuous Lyapunov equation solution
* [[lyapchol]]	Square-root solver for continuous-time Lyapunov equation
* [[dlyap]]	Solve discrete-time Lyapunov equations
* [[dlyapchol]]	Square-root solver for discrete-time Lyapunov equations
* [[care]]	Continuous-time algebraic Riccati equation solution
* [[dare]]	Solve discrete-time algebraic Riccati equations (DAREs)
* [[gcare]]	Generalized solver for continuous-time algebraic Riccati equation
* [[gdare]]	Generalized solver for discrete-time algebraic Riccati equation
* [[ctrb]]	Controllability matrix
* [[obsv]]	Observability matrix
* [[ctrbf]]	Compute controllability staircase form
* [[obsvf]]	Compute observability staircase form
* [[gram]]	Controllability and observability Gramians
* [[gramOptions]]	Options for the gram command
* [[bdschur]]	Block-diagonal Schur factorization
* [[norm]]	Norm of linear model

