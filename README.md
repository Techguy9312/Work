

<?php
// Initialize the session
session_start();
 
// If session variable is not set it will redirect to login page
if(!isset($_SESSION['username']) || empty($_SESSION['username'])){
  header("location: login.php");
  exit;
}
?>
 
<!DOCTYPE html>

<div class="page-header">
        
    </div>

<h1>Hi, <b><?php echo $_SESSION['username']; ?></b>. </h1>

<form action="liftuse.php" method="post" />
<p>Name: <input type="text" name="Name" required /></p>
<p>Dept: <input type="text" name="Dept" required /></p>
<p>Reach Number: <input type="text" name="Reach_Number" required /></p>

Leaks – Hydraulic Oil Engine Oil and Battery:

<span style="color: white;">---------------------------------------------------</span>
<input type="radio" name="Leaks" required
<?php if (isset($Log) && $Leaks=="OK") echo "checked";?>
value="OK">Ok
<input type="radio" name="Leaks" 
<?php if (isset($Log) && $Leaks=="FAIL") echo "checked";?>
value="FAIL">Fail

<br>
<br>

Forks – Top Clip Retaining Pin and Heel – Condition:

<span style="color: white;">-----------------------------------------</span>
<input type="radio" name="Forks" required
<?php if (isset($Log) && $Forks=="OK") echo "checked";?>
value="OK">Ok
<input type="radio" name="Forks" 
<?php if (isset($Log) && $Forks=="FAIL") echo "checked";?>
value="FAIL">Fail

<br>
<br>

Rails, Toe boards and Safety Chains in place:

<span style="color: white;">---------------------------------------------------</span>
<input type="radio" name="Rails" required
<?php if (isset($Log) && $Rails=="OK") echo "checked";?>
value="OK">Ok
<input type="radio" name="Rails" 
<?php if (isset($Log) && $Rails=="FAIL") echo "checked";?>
value="FAIL">Fail

<br>
<br>

Hydraulic Hoses, Mast Chains and Stops – Check Visually:

<span style="color: white;">---------------------------------</span>
<input type="radio" name="HydraulicHoses" required
<?php if (isset($Log) && $HydraulicHoses=="OK") echo "checked";?>
value="OK">Ok
<input type="radio" name="HydraulicHoses" 
<?php if (isset($Log) && $HydraulicHoses=="FAIL") echo "checked";?>
value="FAIL">Fail

<br>
<br>

Overhead Guard – Attached and not Broken:

<span style="color: white;">----------------------------------------------------</span>
<input type="radio" name="Overhead" required
<?php if (isset($Log) && $Overhead=="OK") echo "checked";?>
value="OK">Ok
<input type="radio" name="Overhead" 
<?php if (isset($Log) && $Overhead=="FAIL") echo "checked";?>
value="FAIL">Fail

<br>
<br>

Safety Warnings Stickers – Attached (Refer to Parts Manual):

<span style="color: white;">------------------------------</span>
<input type="radio" name="SafetyStickers" required
<?php if (isset($Log) && $SafetyStickers=="OK") echo "checked";?>
value="OK">Ok
<input type="radio" name="SafetyStickers" 
<?php if (isset($Log) && $SafetyStickers=="FAIL") echo "checked";?>
value="FAIL">Fail

<br>
<br>

Battery Restraint System- Latched:

<span style="color: white;">-----------------------------------------------------------------</span>
<input type="radio" name="BatteryRestraint" required
<?php if (isset($Log) && $BatteryRestraint=="OK") echo "checked";?>
value="OK">Ok
<input type="radio" name="BatteryRestraint" 
<?php if (isset($Log) && $BatteryRestraint=="FAIL") echo "checked";?>
value="FAIL">Fail

<br>
<br>

Battery – Water (fill every 2 weeks/check log):

<span style="color: white;">---------------------------------------------------</span>
<input type="radio" name="BatteryWater" required
<?php if (isset($Log) && $BatteryWater=="OK") echo "checked";?>
value="OK">Ok
<input type="radio" name="BatteryWater" 
<?php if (isset($Log) && $BatteryWater=="FAIL") echo "checked";?>
value="FAIL">Fail

<br>
<br>

Operator’s Manual in Container:

<span style="color: white;">---------------------------------------------------------------------</span>
<input type="radio" name="OperatorManual" required
<?php if (isset($Log) && $OperatorManual=="OK") echo "checked";?>
value="OK">Ok
<input type="radio" name="OperatorManual" 
<?php if (isset($Log) && $OperatorManual=="FAIL") echo "checked";?>
value="FAIL">Fail

<br>
<br>

Capacity Plate and Warning Placards Attached and Legible:

<span style="color: white;">--------------------------------</span>
<input type="radio" name="CapacityPlate" required
<?php if (isset($Log) && $CapacityPlate=="OK") echo "checked";?>
value="OK">Ok
<input type="radio" name="CapacityPlate" 
<?php if (isset($Log) && $CapacityPlate=="FAIL") echo "checked";?>
value="FAIL">Fail

<br>
<br>

Motor or Battery Restraint System - Adjusted and Latched:

<span style="color: white;">----------------------------------</span>
<input type="radio" name="Motor" required
<?php if (isset($Log) && $Motor=="OK") echo "checked";?>
value="OK">Ok
<input type="radio" name="Motor" 
<?php if (isset($Log) && $Motor=="FAIL") echo "checked";?>
value="FAIL">Fail

<br>
<br>

Seat Belt/Harness, Buckle and Retractor – Functioning Smoothly:

<span style="color: white;">-------------------------</span>
<input type="radio" name="SeatBelt" required
<?php if (isset($Log) && $SeatBelt=="OK") echo "checked";?>
value="OK">Ok
<input type="radio" name="SeatBelt" 
<?php if (isset($Log) && $SeatBelt=="FAIL") echo "checked";?>
value="FAIL">Fail




<br>
<br>

<input type="submit" value="Submit" />
</form>

<br>
<br>

<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Welcome</title>
    <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.css">
    <style type="text/css">
        body{ font: 14px sans-serif; text-align: center; }

.page-header {
  padding-bottom: 20px;
  height:320px;
  margin: 0px 0 20px;
  border-bottom: 5px solid #eee;
  background-image: url("https://github.com/Techguy9312/Techguy9312.github.io/raw/master/safety.png")
}

    </style>
</head>
<body>
    
    <p><a href="logout.php" class="btn btn-danger">Sign Out of Your Account</a></p>
</body>
</html>
