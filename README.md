# OOAD-WEEK08

## Use Case Diagram (ภาษาไทย)
* รูปที่ 1 การจอง ยืม คืน หนังสือ

code

Jonh -down- (reserve DVD)
Jonh -down- (borrow DVD)
Jonh -down- (return DVD)
(reserve DVD) --|> (check reseervation) : include
(borrow DVD) --|> (check reseervation) : include
(calculate fine) -up-|> (return DVD) : entend

[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/ZOux3eCm44HxJZ4b55m0HLHK722zMGPXOQsbZPqq73uWX0Ifqhxvzd5Mr3LAuuls9hfdLnNzIOTe5Zy_4CQKJGzw2sxosgAKcRBW45poKIiqW5S9UMHnBVqlS1t4Ozq_Y0kIWql4v9MxdPgeunS0)

* รูปที่ 2 ระบบส่วนลดลูกค้า

code

:admin user:as user
:simple user: as mysql
user <-up- mysql : entend
user -right- (Add Discounted customer)
mysql -right- (Add simple user)
(Add simple user) .right.> (send a email) : include
(Add Discounted customer) ..> (send a email) : include

[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/VOwn2iCm34HtVSMDoU1yW8T0eJzYB0q2oschUEZVrpYq15gw7E9Et3kAhdOhWkRoG4HosDFlXOOY14mNPfoUPlfoi2mh9fVAI11BMkPUfJMNna8niMaz0SP5GqDO3rvFfEwzuUqVtAjwtbeF6Bdvljc7_olvk-C5) 

* รูปที่ 3 ลูกค้ากับตู้ATM

code

:card holder: as holder
holder -- (enter password)
holder -- (check Balance)
holder -- (withdraw Cash)
holder -- (Get Slip)

[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/iqfEB4fHoCZFIKajKh1II2o6ihcWGhgw2XgfUIL0La5YSN5vVb6A9h9KSaPgShQ2Ks9EObvoAefCUMP9HafHOhc2Ss9n1egCUsg9Gd1EPe4c0000) 

* รูปที่ 4 การสั่งซื้อสินค้าทางโทรศัพท์ 

code

left to right direction
Customer -- (Check Status)
Customer -- (Place Order)
Customer -- (Fill Order)
Customer -- (Establish Credit)
salesperson -up- (Check Status)
salesperson -up- (Place Order)
Clerk -up- (Fill Order)
Manager -up- (Establish Credit)

[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/RSqn3i8m38NXFQVmI8UU8e8DWSG9J68QgoP1jdl_aWbAMT_tf5_euU0DbAVYa5afERSQucBUdgG0umY7L2ZDS7FqnOQFTReA9eABPj8VER78NpYQurtO2aIbp3w4RQ2V38NiHMgjGjX4zleLwXY5T7xFkqp7CrQSI5S0)

* รูปที่ 5 ระบบการลงทะเบียน

code

:Registration Staff : as staff
:Financial Staff : as mysql
staff -- (Register Course)
Student -- (Register Course)
(Register Course) --|> (Checkout Course) : uses
Student -- (Record Billing)
mysql -- (Record Billing)

[![IMAGE ALT TEXT](http://www.plantuml.com/plantuml/img/ROyn2iCm34Ltd-AFoP0BUEZGG0yGdy0uIYfgPB3ahOTlcq19QHOX_d_YeM1j9Z4C0pfCjB8QLOobLQNUXKCxKIfrnfLpPbbxvt5ZYP8uPWIBo-8H5VhPt3PFh_ubR-nvGJVUAJrAis_iqPJK-PslqRZ8Bi9cEkRk1phzvGK0)
 

