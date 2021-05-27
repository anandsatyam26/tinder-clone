"# tinder-clone" 
npx create-react-app tinder-clone
del 'App.test.js', 'logo.svg', 'setupTests.js'
cd tider-clone
npm instal
open new terminal 
cd tnder-backend
npm install
now we need to set entry point of server.js in backend's package.json
under package.json, under "main" add "type":"module" and under "test" add "start":"node server.js"
open postman (interact with servers backend stuff) in local to check our API if they are working correctly - get new "+" tab, and type the http://localhost:8001/ and http://localhost:8001/tinder/cards - post http://localhost:8001/tinder/cards -> body -> raw -> JSON - add below:

    [
    {
    "name": "Elon Musk",
    "imgUrl":
    "https://www.biography.com/.image/t_share/MTY2MzU3Nzk2OTM2MjMwNTkx/elon_musk_royal_society.jpg"
    },
    {
    "name": "Jeff Bezoz",
    "imgUrl":
    "https://www.biography.com/.image/t_share/MTY2NzA3ODE3OTgwMzcyMjYw/jeff-bezos-andrew-harrer_bloomberg-via-getty-images.jpg"
    }
    ]

    [
    {
    "name": "Elizabeth Olsen",
    "imgUrl":
    "https://www.gstatic.com/tv/thumb/persons/620481/620481_v9_bb.jpg"
    },
    {
    "name": "Scarlett Johansson",
    "imgUrl":
    "https://pm1.narvii.com/6310/c0e449205abaa82b4c37b3baf0e77ab95fe13137_00.jpg"
    },
    {
    "name": "Gal Gadot",
    "imgUrl":
    "https://upload.wikimedia.org/wikipedia/commons/5/5b/Gal_Gadot_cropped_lighting_corrected_2b.jpg"
    }
    ]


set GET to http://localhost:8001/tinder/cards again and check in postman, we get the things we just post

After that go MongoDB and check collections, all data are there

