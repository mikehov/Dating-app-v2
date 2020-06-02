# Read me :)

## Concept Dating-app
_When I'm chilling in my room listening to my music playlist, I want to be notified that I have a match, so I can see who it is and maybe get to know them._

This dating-app is about the feature "swiping" and "notifications". Its a casual dating-app with swiping people to the left if your not interested or to the right if you are interested. You will get a notification if you have a match.

## Installing the Dating-app project
1. Download or Clone my repository and set it up in te correct folder. 
2. Go to your terminal and go to the correct folder. (tip: use `pwd` and `cd` to do so.)
3. Install npm by typing `npm install`.
4. To run the project, type: `nodemon index.js` or `npx nodemon index.js`.

## Documentation
To find the documentation, check out my wiki page of my repository. 
https://github.com/mikehov/Dating-app/wiki

## Data structure
| **Data**           | **Value**                      | **Type**         |
|--------------------|--------------------------------|------------------|
| _id                | randomIdCode                   | objectID         |
| firstname          | Melanie                        | String           |
| lastname           | Brinkhaltes                    | String           | 
| email              | melaniebrinkhaltes@outlook.com | String           | 
| gender             | female                         | String           | 
| age                | 22                             | Int32            | 
| city               | Zaandam                        | String           | 
| characteristics    | 0:excited, 1:happy, 2:godess   | Array            | 
| picture            | photo-melanie.png              | String           | 
| likes              | userid1:1, userid2:0,          | Object           | 


## Sources
AWS Simplified. (2020, February 10). SQL vs NoSQL Explained [Video file]. YouTube. Retrieved from https://www.youtube.com/watch?v=ruz-vK8IesE&t=310s

Bitovi. (n.d.). Tinder Carousel | intermediate recipes | Guides | CanJS — Build CRUD apps in fewer lines of code. Retrieved June 2, 2020, from https://canjs.com/doc/guides/recipes/tinder-carousel.html

Box Shadow CSS Generator | CSSmatic. (n.d.). Retrieved May 10, 2020, from https://www.cssmatic.com/box-shadow 

Claire is seasoned technical writer, editor, and HTML enthusiast. She writes for HTML.com and runs a content agency, Red Robot Media. (n.d.). Attribute for METHOD = GET | POST. Retrieved May 26, 2020, from https://html.com/attributes/form-method/

de Vries, D. (n.d.-a). lecture-3. Retrieved June 2, 2020, from https://docs.google.com/presentation/d/1PJTtYNOFw8n9Zr54kBiabNpb777QDMNJIFt0bKVR__Q/edit#slide=id.g4e3b0a74b9_1_416

freeCodeCamp.org. (2018, October 25). Let’s Build a Tinder-Like Swipe Carousel [Video file]. In YouTube. Retrieved from https://www.youtube.com/watch?v=Iz6W4HizXq8
```
Code
```

de Vries, D. (n.d.). lecture-4. Retrieved June 2, 2020, from https://docs.google.com/presentation/d/1J0SVcx7rMnFp37JqsQMHQq92EfBRUFdgSAj5i9wQKjg/edit#slide=id.g85a98fc989_0_63
```
Code
```

MongoDB. (n.d.-b). Managed MongoDB Hosting | Database-as-a-Service. Retrieved June 2, 2020, from https://www.mongodb.com/cloud/atlas

MongoDB. (n.d.-b). Connect to MongoDB. Retrieved June 2, 2020, from https://docs.mongodb.com/guides/server/drivers/

Sarzyński, Ł. (n.d.). fill HTML forms without JavaScript. Retrieved May 26, 2020, from https://dev.to/lukaszsarzynski/fill-html-forms-without-javascript-4d24

SVG drop shadow using css3. (2011, May 22). Retrieved May 10, 2020, from https://stackoverflow.com/questions/6088409/svg-drop-shadow-using-css3

Code from the student Rowin Ruizendaal:
```
app.post("/matches", function (req, res) {
  db.collection('Users').find() 
    .toArray(function (err, data) {
      if (err) console.log(err);
      // console.log(data);
      let allIds = [];
      for (let i of data) {
        allIds.push(i._id);
      }
      console.log(allIds[index]);
      index++;
      console.log('Dit is de index' + index)

      if (index == allIds.length) {
        index = 0;
      }

      console.log(data[index]);
      console.log(req.body)

      // Random distance counter
      let randomDistance = Math.floor(Math.random() * 100);
      data[index].randomDistance = randomDistance;
      console.log(data);
      res.render('swipe.ejs', {
        data: data[index]
      }); 
    });
});

function add(req, res) {
  data.push({
    fullname: req.body.fullname,
    age: req.body.age,
    description: req.body.description,
  });

  res.redirect('/list');
}

mongodb.MongoClient.connect(uri, {
    useUnifiedTopology: true,
  },
  function (err, client) {
    if (err) throw err;
    db = client.db(process.env.DB_NAME);
    console.log('Connected to database')
  });
```

#### Pictures
Christopher, T. (2017, May 21). Toby Christopher [Photo]. Retrieved from https://unsplash.com/photos/P-CeaGknSJA

Hefitiba, T. (2018, February 5). Toa Heftiba [Photo]. Retrieved from https://unsplash.com/photos/O3ymvT7Wf9U

Hiles, S. (2017, December 26). Sonnie Hiles [Photo]. Retrieved from https://unsplash.com/photos/gG70fyu3qsg

Jensen, D. (2017, August 15). Daniel Jensen [Photo]. Retrieved from https://unsplash.com/photos/tQpypKA92k8

Kobalasingam, H. (2018, November 8). Harishan Kobalasingam [Photo]. Retrieved from https://unsplash.com/photos/8PMvB4VyVXA


