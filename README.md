# Playlist Maker
Authors: [Vishal Gondi](https://github.com/vgondi123), [Rachel Danover](https://github.com/RDanover), [Mariam Golwalla](https://github.com/mgolw001), [Seokha Kang](https://github.com/seokhakangcs)

## Phase 1 - Project Description

### Importance of the Project
Our Project is a Playlist maker where the user can add and delete songs to various playlists. We are interested in this project in particular as we all really like to listen to music, so this seems like a project we would enjoy building to kind of learn the code and algortithms behind our favorite streaming services.

### Language
We are going to be using C++ as our language for the project.

### Tools & Technologies
We are going to use Vim, Visual Studio, Xcode. All inputs and outputs will take place in the terminal.

### Inputs & Outputs
The user will input the song name and artist, and the playlist they created will be outputted. The songs will not actually play but will instead say "Now playing \<insert songname>\."

### Feature
Users can also choose to play their entire playlist, shuffle play their playlist, and hide songs to keep them from playing. In addition, they will be able to name the playlist and have the option to see a summary of their music habits (similar to Spotify Wrapped). Our songs will be held in a vector as pointers make it convenient to add and remove songs, and to change the order for the shuffle feature.

## Phase II

###Class Diagram
![Screenshot (12)](https://user-images.githubusercontent.com/60625627/143936351-66a09c81-0aee-4b09-80af-cbb76e6b7e02.png)

### Description of diagram
Our project will feature two interfaces, one where the user can see their playlists and choose to delete them or add more, this is also where users will access their playlists. This interface will hold a vector of playable pointers making it a composition of the playable class, a playlist can have one user but a user can have 0 to any positive integer number of playlists. Our second interface will be the playlist interface which will allow users to play the songs in their playlist, delete songs, hide them, or add new ones, they will also be able to view analytics about their listening habits if they choose to have their data collected. This interface will feature two vectors composed of playable object pointers making the playlist class a composition of the playable class. The song class is simply a leaf class and will not be directly accessed by the user. A playlist can have 0 to many songs, however (with our implementation) a song will only belong to one playlist. 
 
 ## Phase III
 ### Composite Pattern:
 We chose this pattern as it seemed to best to use with the structure of our project. A playlist is traditionally made up of many songs which is a composition. By using    this design pattern we can have more structural code. It also makes it easier for users to interact with playlists and songs as they are treated the same under the composite pattern. We used composition in both the User_Menu class and in the playlist class to help with organization. 
### Abstract Factory:
 We chose this pattern to solve the ethical issue of collecting data without user consent. We will prompt the user if they would like their data to be collected for use in     displaying their anaylitics. If the user opts out, their data will not be collected and an alternative implementation of playlist and song will be used. By using this     pattern it simplifies and organizes the design by splitting the creation of certain functions based on the user's decision. 

  ## Final deliverable
 
 ### Screenshots
![Screenshot (15)](https://user-images.githubusercontent.com/60625627/143972904-eacd16d4-ee59-4c91-a654-5575ec78f545.png)
![Screenshot (16)](https://user-images.githubusercontent.com/60625627/143972914-cc741241-1eff-4077-b976-da9b91fa24be.png)
![Screenshot (17)](https://user-images.githubusercontent.com/60625627/143972920-1b19911f-1d0c-427d-a1bb-5e95c42b1a60.png)
![Screenshot (18)](https://user-images.githubusercontent.com/60625627/143972930-87a7b633-fc04-48c8-87cc-f77ab4cf814e.png)
![Screenshot (19)](https://user-images.githubusercontent.com/60625627/143972943-6c542ef1-a931-4068-8a56-4826a85ecb25.png)
![Screenshot (20)](https://user-images.githubusercontent.com/60625627/143972955-4872bd9c-63df-4572-8287-24fe7a112726.png)

### Installation/Usage
 To use our project click the code button and copy the url, you can then clone the repository into an IDE of your choosing. If you are using hammer use the command "git clone --recursive \<githuburl\>". Once you have a copy, enter into the directory and type "cmake3 ." followed by "make" then to run the program type "./output". To interact with the program type your responses into the keyboard and hit the enter key when you have finished typing your response. Please enjoy our playlist program. 
 
 ### Testing
Our program was tested via a test.cpp file which contained a second main function containing various tests for all of our functions. For some functions, special test functions were made to avoid having to ask for input while running tests. 
![Screenshot (13)](https://user-images.githubusercontent.com/60625627/143936770-b34a860a-dde6-464d-badd-4165732d751e.png)
![Screenshot (14)](https://user-images.githubusercontent.com/60625627/143936785-4747510f-c185-406e-af4b-4c0d184a4b12.png)


 
