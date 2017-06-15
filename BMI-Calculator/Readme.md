# BMI Calculator

BMI or Body Mass Index, is a calcualtion to determine if you are overweight. 

Please take notes on the following data:

Formula for BMI

 `weight/( height )^2`
 
 BMI is done using Meters, and KG, so most users will need help calculating this:
 
 1 Meter = 3.28084 FT
 
 1 Killogram = 2.20462 Lbs
 
 
 In the Sample, I have a Converter - While we can just do it ourselves, lets do it a longer way, so the user is more engaged.
 
 

Private Sub Command1_Click()
    Label4.Caption = BMI(Text1.Text, Text2.Text)
End Sub

Private Function BMI(height, weight)
      BMIValue = (weight) / (height ^ 2)
      BMI = Format(BMIValue, "0.00")
End Function
