# Your Turn!

### For your task, you will be creating a basic drivetrain class.

#### Try not to copy code! If you find code online, type it out!


- [ ] Complete Step 1 on the README
- [ ] create 4 `WPI_TalonSRX` Motors with different CAN ID's.
  - This may require an import of the CTRE Library
  - Make sure you use `WPI_TalonSRX` not `TalonSRX` as it is compatible with `SpeedControllerGroup`.
  - The CAN ID's should be defined as constants
- [ ] create an instance of the XboxController class
  - [ ] Use a `SpeedControllerGroup` for each side of the robot
  - We are not following the front motors! Make sure you look up `SpeedControllerGroup` in the docs.
- [ ] create an instance of the DifferentialDrive class
  - [ ] We are passing in the 2 `SpeedControllerGroup`'s we just created
- [ ] Reset all four motors to factory `RobotInit`
- [ ] Read from the XboxController in `TeleopPeriodic`. Make sure you look up `XboxController` and `GenericHID` for this part.
  - [ ] Pass in values from a joystick on the controller to the `ArcadeDrive` method from the `DifferentialDrive` drivetrain we just created
  - [ ] Make a conditional statement that voids both the X and Y direction of a joystick if they are less than `0.05` or greater than '-0.05' (turns it into `0`).


If you get stuck,

+ *Read the error messages*
+ Look at previous code examples (Hint: some projects in the past have used `SpeedControllerGroup`)
+ Look at the [CTRE](https://www.ctr-electronics.com/downloads/api/cpp/html/index.html)
 and [WPILib](https://first.wpi.edu/FRC/roborio/release/docs/cpp/) documentation
+ Ask a friend
+ Ask a student leader

