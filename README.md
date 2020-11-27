
## Milestone 3 project

# Self isolation watch
'Self isolation watch' is designed to help people keep track of their symptoms and see what other users' symptoms are. They can add a symptom, description and the date they started feeling this way. 
This will help them keep note of their potential retraction of the virus as well as give them an indication into how contagious they are. Users will be able to create a profile, where they save their symptoms, update them accordingly and when they are no longer symptomatic, they can delete them.' 

## Main Aims 
- To create an app that gives people a platform to share their symtpoms and learn about each others.
- Take the pressure of a person to remember when they started feeling this way. 

## User Stories 
 
- 'As a recent self isolater, I want to keep track of what symtpoms I have and how long I have had them, so that I have more information to give to the doctor.'

- 'As a key worker, I want to browse through patients' symptoms, so that I can speed up diagnosis. '

- 'As a recent self isolater, I want to update the symptoms I have had, so that I can find out how far from recovery I am.'

- 'As a recent self isolater, I want to read through other peoples symptoms and compare, so that I can find out if my symptoms are typical.'


## Personnas 
- 'Someone at work has recently tested positive for covid-19, we must self isolate and track our symtoms (if any), I spend all day on my laptop, if only there was an app where i could record my symptoms and the date i started feeling the symptoms too!' (Evelyn, 31, mother of 2 children under 5)

- 'Its so frustrating when patients come to me saying that they feel ill and they think they have COVID, but no note of when they started feeling ill! I wish they would bring me more information' (Jocelyn, 55, Nurse) 

- 'I feel terrible, but I dont know if its just a flu.. I want to know if my symtpoms are from COVID or something else. Im conscious of all the fear mongering and fake news out there..' (Luke, 28, Marketing manager)




## Bugs discovered

- Refresh causing null data input

* Everytime I was refreshing the page and logged in, a new input which was blank was being added to my mongo db. It was then also showing up on my page, as I was displaying all mongo.db entries. 

### solution:

- Materialize Code not displaying 

* I had added some code from a meaterialize carousel and it wasnt showing up on my page.
* I tried to chnage the colour of the text and double checked that I wasnt pasting within any none relevant for loops etc. 

### solution:





## Testing

Please view the complete testing process in this separate document [here]().

## Deployment

This project was developed using Gitpod as the chosen IDE and GitHub as a remote repository. 

The deployed project can be viewed on the following link: 

The project's GitHub repository can be viewed with the following link: 

### Local deployment

If you would like to work on this project further you can clone it to your local machine using the following steps:

1. Scroll to the top of this repository and click on the "clone or download button"
2. Decide whether you want to clone the project using HTTPS or an SSH key and do the following:
    * HTTPS: click on the checklist icon to the right of the URL to copy it
    * SSH key: first click on 'Use SSH' then click on the same icon as above
3. Open a new Terminal window in your IDE of choice
4. Change the current working directory to the location where you want the cloned directory.
5. Enter the following command and press 'Enter' to create your local clone:
```
git clone 
```

6. Now create a Database that you intend to use for this cloned project with MongoDB.
7. Return to the Terminal and enter the following to install all required dependencies:
```
pip3 install -r requirements.txt
```
8. Create an env.py file with the following content, replacing the 'username','password', 'cluster_name' and 'database_name' with your MongoDB database values:
```
import os

os.environ["MONGO_URI"] = "mongodb+srv://<username>:<password>@<cluster_name>-ocous.mongodb.net/<database_name>?retryWrites=true&w=majority" 
```
9. Add your env.py file to .gitignore to make sure your database information is not viewable to others
10. Your cloned version is now ready to run locally with the following command:
```
python3 app.py
```

You can find both the source of this information and learn more about the process with the following link: [Cloning a Repository](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository)

### Deploying this project to Heroku 

To deploy the project to Heroku, I used the following steps:

1. I created a Heroku account, signed in and created a new app with a unique name that had not already been taken (this project uses ' '). I then set the region to the closest to me: 'Europe'.
2. With the app created, I went to the 'Settings' tab and clicked the 'Reveal Config Variables' button. From here, I input the following values:
```
MONGO_URI: mongodb+srv://<username>:<password>@<cluster_name>-ocous.mongodb.net/<database_name>?retryWrites=true&w=majority
IP: 0.0.0.0
PORT: 5000
```
(Note: within the MONGO_URI value, I replaced the 'username','password', 'cluster_name' and 'database_name' with my specific database values. They are kept private for security reasons.)


3. In Gitpod, I created a requirements.txt file with the following command:
```
pip3 freeze --local > requirements.txt
```
4. I then created a Procfile with the following content within (making sure that 'Procfile' was written with a capitalized 'P'):
```
echo web: python app.py > Procfile
```
5. I then committed and pushed these new files with the following:
```
git add -A
```
```
git commit -m ""
```
```
git push
```
6. With these files committed and pushed, I navigated to the deployment tab on heroku.

7. I then clicked 'github' on the deployement method row.

8. When prompted, i typed the name of my git hub repo into the search box, ('self-isolation-watch') 

9. When my repo appeared I clicked it.

10. I then scrolled down towards the deploy button and clicked 'enable automatic deployment'.

11. finally i clicked deploy! 

12. to ensure that my app had successfully been deployed i clicked open app and saw the text 'hello world' which i had used as a test and returned within my first view in my app.py folder. 


This completed the process of deploying the project to Heroku. Once deployed, I continued to push all changes made to the project to Heroku throughout the remaining development process.

## Credits

### Content

The content of this website is entirely fictional and written by myself.

### Images
![background image by sarah kilian](https://unsplash.com/photos/yvxw4K9lYKo)



### Acknowledgements

Thank you to the following people who helped with support and inspiration:
[Nick bell] 
[Miranda] 


### credits
