# Forward-and-Inverse-Kinematics-of-3DOF
***************

![IMG_2303](https://github.com/user-attachments/assets/f8f2235b-6b63-4e27-a703-b41570247211)

*************
## FOEWARD 
**************
<b1><b1>
x = L1 cosθ1 + L2 cos(θ1+θ2) + L3 cos(θ1+θ2+θ3) <br>
y = L1 sinθ1 + L2 sin(θ1+θ2) + L3 sin(θ1+θ2+θ3) <br>
θ = θ1+θ2+θ3 <br>
<br> <br> <br>

********************* 
## INVERSE 
*****************
<br><br>
(x3,y3,L1,L2,L3) <br>
θ1,θ2,θ3 = ? <br>

x2 = x3 - L3cosθ <br>
y2 = y3 - L3sinθ <br>

cosθ2 = x2^2 + y2^2 - L1^2-L2^2/ 2 * L1 * L2

x2 = L1 cosθ1 + L2 cos(θ1+θ2)<br>
y2 = L1 sinθ1 + L2 sin(θ1+θ2)<br>

x2 = cosθ1 (L1+L2 cosθ2) - sinθ1 (L12 sinθ2)<br>
y2 = cosθ1 L2 sinθ2 + sinθ1 (L1 + L2 cosθ2) <br>

cosθ1 = ( (L1 + L2 cosθ2)x2 + L2 sinθ2 y2) / x2^2 + y2^2 <br>
sinθ1 = L1+L2cosθ2 * y2-L2 sinθ2 x2/ x2^2 + y2^2 <br>

cosθ1 = sinθ1 / cosθ1 <br>
θ1 = tan^-1 (sinθ1 / cosθ1) <br>
θ3 = (θ1 + θ2) <br><br><br>


