# Changelog

### 1.1.5

Fixed:      Nasty bug where step data was being deleted....

### 1.1.4

Fixed:      Wizard createModel now only returns the model and sets model data in onModelCreated (1.1.1 but properly)
Changed:    onModelCreated moved below createModel

### 1.1.3

Revert:      revert #9 / 1.1.1. Unit test still fixed.

### 1.1.2

Fixed:       set model steps before giving data

### 1.1.1

Fixed:      Wizard createModel now only returns the model and sets model data in onModelCreated
Fixed:      Broken unit test

### 1.1.0

Added:      Method to share data completely between one ore more steps (see documentation)

### 1.0.6

Changed:    Lifecycle methods only called now if the step is actually changing to a different step.

### 1.0.5

Added:      New hooks onLeavingStep and onLeftStep in the Wizard
Changed:    $stepData on StepModel is now public so steps can modify the step data (with caution!)      

### 1.0.4

Added:      Documentation!

### 1.0.3

Changed:    Removed void return type from `loadDataFromPersistentState()` to support PHP < 7.1

### 1.0.2

Changed:    `onLeaving()` and `onLeft()` functions now take the `$nextStepName` as a parameter.

### 1.0.1

Added:      To allow for methods to be called before changing a step - `onLeaving()` and `onLeft()` methods to `Step`.
`beforeChangeStep()`, `afterChangeStep()`, `createSteps()` to Wizard. 

Changed:    `getSteps()` modified to return `$this->steps`, which it will set (using `createSteps()`)if it is null. 

### 1.0.0

Added:      Changelog
