# CSC-560-Unit-3-API

Applied Restful API & Integration
CSC 560
Dr. Litman

 Unit 3
API
August – October 2022

Andrea M. Tadlock
CUW ID - F00530415
09/25/2022
 
As I was struggling through the Unit Test Assignment, I decided I needed to find a simpler CRUD API example for me to understand each module. Sometimes doing assignments it is easy to follow steps and lose sight of what is happening. Finding a simpler example allowed me to focus on the modules. The assignment took me 12 hours to work through mostly because I wanted to focus on each module and feel more comfortable with them. While I am still grasping how the bodyParser package works, I am understand with more confidents the modelling, routing and controlling components. One of my annoyances is the need for the mongoose package to force plural and lowercase for a collection. After a deeper dive, I had to explicitly name the collection from my database in the model component, and all was good. Numbers were interesting as well. I struggled with the want to use Decimal128 or keep it simple for now with Numbers as a type. In the end, I thought let’s continue with keeping the code simple to help me learn how everything works. One of my queries added a twist, it was not quite easy for me to get the actual document counts for the number of players who played 50 games or more. Once I understood the syntax for “countDocuments,” I was able to proceed.

The class has been very much a learning experience and is helping me grasp the interworking of RESTful APIs.

To help with the assignment, I included in my Repository the Player List to build the collection. While I am sure the code is very readable to identify everything needed, I think the below will add some value when verifying code:
Database: 76erBasketballDB
Collection: Players
List of Players: Players-List.json

URL 
Create Player: 		Post http://localhost:8080/create
Update Player:  		Post http://localhost:8080/player/playerid , where playerid is the key from the collection
Delete Player: 		Delete http://localhost:8080/player/playerid , where playerid is the key from the collection
Full Collection List: 	Get http://localhost:8080/get-all
Find Single Player: 	Get   http://localhost:8080/player/playerid , where playerid is the key from the collection

Five Queries
1.	All Players Sorted by the player with the highest 3 point average per game to the lowest
a.	Get http://localhost:8080/get-all-sort

2.	Player with the Highest Game Point Average
a.	Get http://localhost:8080/high-scorer
3.	Player with the Least Number of Personal Fouls per Game
a.	Get http://localhost:8080/least-fouls
4.	The Number of Players who played more than 50 Games
a.	Get http://localhost:8080/fifty-plus
5.	The List of Players who Averaged 20 Points or More a Game and Averaged 2 or More Assist per Game
a.	Get http://localhost:8080/twenty-two 
		

