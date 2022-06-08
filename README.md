# WarhammerWebsite
creation of new website for store league


## Database objects:
### User(object)
userName(string) - contains the username of the user

screenName(string) - contains the name that other users see of the user

password(string) - the users password to log in


### map(object) - contains all hexObj
#### hexObj(object) - an indivudual hex. 
L(int) : coordinate left 

R(int):coordinate right 

H(int) : coordinate horizontal

occupyingForceBool(boolean) : true if occupied, false if empty

occupiyingForce(string): name of the army on the square, if any

