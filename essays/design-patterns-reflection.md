---
layout: essay
type: essay
title: "Reflection on Design Patterns"
# All dates must be YYYY-MM-DD format!
date: 2024-04-25
published: true
labels:
  - Design Patterns
  - Efficiency
  - Consistency
  - Communicability
---

## What are Design Patterns? 

In my opinion, design patterns in code are similar to using keyboard shortcuts. They are easily replicable, and they make coding much more convenient. They expedite the process of working on code just like how keyboard shortcuts expedite working on documents. Design patterns allow for code that would have to be typed out multiple times to be types just once and called multiple times. This is mostly commonly seen in methods and functions in code to allow easy replication of code in multiple places. Design patterns also allow for better consistency to be used in code. An example of this would be objects and classes. Creating objects and components in code and accurately describing how they work is helpful for keeping consistency in coding, because it makes sure they’re organized. This organization also lets multiple people work on the same code without it being overly difficult to understand. If multiple people can understand how one object works, they can understand how they all work. This is similar to if multiple people were working on a spreadsheet, if they all understood how to make use of certain keyboard shortcuts, they could all work with much greater efficiency than if they didn’t. The consistent code allows for programmers to create a solid foundation for which their code is built upon. One more aspect of design patterns is their communicability. Design patterns allow for code to be more easily understood, which means that they can be more easily explained from developer to developer. This mirrors key shortcuts, because it is very easy to explain them to new people. Explaining copy and paste shortcuts to others is very easy, and massively improves efficiency when working on a document or spreadsheet. Design patterns like methods are very similar and can be easily explained as well. 

## How do I use Design Patterns? 

```
<Card className="h-100">
    <Card.Header>
      <Image src={student.image} width={75} />
      <Card.Title>{student.firstName} {student.lastName}</Card.Title>
      <Card.Subtitle>{student.address}</Card.Subtitle>
    </Card.Header>
    <Card.Body>
      <ul className="list-group list-group-flush">
        <li className="list-group-item">Description - {student.description}</li>
        <li className="list-group-item">My Interests - {student.interests}</li>
        <li className="list-group-item">
          <a href={student.resume} className="btn btn-primary">My Resume</a>
        </li>

      </ul>

      <ListGroup variant="flush">
        {notes.map((note) => <Note key={note._id} note={note} />)}
      </ListGroup>
      <AddNote owner={student.owner} contactId={student._id} />
    </Card.Body>
  </Card>
```
In this code, a design pattern I used was utilizing a component to display information on my pages. For people and company users, I made multiple components to display the information from them in the way I wanted. For example, seeing a profile on the student home page would be different from seeing that same student’s profile in the recommendations tab. This is because the necessary information for these tabs was different across both of them. The component design patterns allowed me to display information for every student, as long as I had their data. This is very convenient, as it allows me to replicate the necessary information wherever I need it in the website. 

```
class StudentsCollection {
  constructor() {
    // The name of this collection.
    this.name = 'StudentsCollection';
    // Define the Mongo collection.
    this.collection = new Mongo.Collection(this.name);
    // Define the structure of each document in the collection.
    this.schema = new SimpleSchema({
      firstName: String,
      lastName: String,
      address: String,
      image: String,
      description: String,
      interests: String,
      school: String,
      resume: String,
      owner: String,
    });
    // Attach the schema to the collection, so all attempts to insert a document are checked against schema.
    this.collection.attachSchema(this.schema);
    // Define names for publications and subscriptions
    this.userPublicationName = `${this.name}.publication.user`;
    this.adminPublicationName = `${this.name}.publication.admin`;
  }
}
```

Collections were another design pattern I used in my code. In this code, I created the StudentsCollection class to store all the data that I needed from students. This code stores all the student objects in a mongo collection, and allows me to search for them by their unique student id. This is very helpful because it keeps all of my student objects in one place, and ensures that my code stays organized. I did the same with companies as well, to keep track of all of my company objects. Having both students and companies easily accessible makes my code easier to understand not just for me, but for the other students working with me on the project as well. 

## Conclusion

Design patterns are crucial for ensuring that projects stay working, especially in a group setting. Without them, code would become very inefficient and much harder to understand. I would recommend that everyone with an interest in coding to invest some time in learning some design patterns to make sure they write efficient and clean code. 
