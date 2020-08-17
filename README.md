<?php
include_once 'azurroheader.php';
?>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AzurroCheck</title>
</head>
<body>
                <div class="main">
                        <div class="text">
                           <h3>Private site for Azurro Garden owners.</h>
                           <h3>...........................................</h>
             
                        </div>

                        <form action="azurropassword.php" method="POST">

                                  <label for="enterpassword">Pleace, enter password :</label><br>
                                  <input type="text" id="enterpassword" name="enterpassword" placeholder="Enter your password ..."><br>

                                  <input type="submit" id="submitbuton" value="Submit"><br><br>
                        </form>
                        
                        <div class= "password">
                                <?php                       
                                //echo $_POST["enterpassword"];
                                $pass = 'ogi';
                                
                                    if($pass == $_POST["enterpassword"] )
                                    {
                                        //echo "Right password !" ;
                                        header('Location: http://localhost:8080/azurro/index1.php');
                                        //exit();   
                                    }
                                    else
                                    {
                                        echo "Wrong password !";
                                    }
                                ?>
                        </div>

                        
                </div>  
    
</body>
</html>
<?php
include_once 'azurrofooter.php';
?>
</html>
<?php
include_once 'azurrofooter.php';
?>
