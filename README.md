# WarhammerWebsite
creation of new website for store league


## Database objects:
### User(object)
userName(string) - contains the username of the user

screenName(string) - contains the name that other users see of the user

password(string) - the users password to log in

#### armyGroups{object} - contains all armies that the user has

##### Army{object} - the baseline unit that is controlled by the player on the map 

ArmyName (string) - the name of the army

##### unit{object} - contains the individual unit cards and details. the number of units in an army will equal the number of unit objects{ 

unitName (string) - name of the unit

keyWords (string) - contains all unit keywords

unitCost(int) - points cost of the unit

unitCount(int) - # models in the unit

sGT (boolean) - true if the unit has a sergeant

unitEquipment (string) - all standard unit equipment

unitRelics (string) - all relics or relic adjacent upgrades

warlord(boolean) - true if warlord

warlordTrait(string) - contains the warlord trait if the unit has one

psycichPwr(string) - all psychic powers the unit has

##### }



### map(object) - contains all hexObj

#### hexObj(object) - an indivudual hex. 

L(int) : coordinate left 

R(int):coordinate right 

H(int) : coordinate horizontal

occupyingForceBool(boolean) : true if occupied, false if empty

occupiyingForce(string): name of the army on the square, if any


## Website API

### Post : /User/GetUser : retrieves all user information from database
