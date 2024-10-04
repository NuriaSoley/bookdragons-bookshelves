# Project Name

This repository is a [json-server](https://github.com/typicode/json-server) created to feed data into the React Application below.

#### [Client Repo here](https://github.com/Gemma-Fernandez/bookdragons-bookshelves)

# Server Structure

## Collections

### books

```javascript
{
    id,
  title,
  author,
  image,
  published,
  pages,
  summary,
  rating,
  read,
  review,
  authorId,
}
```
### authors

```javascript
 {
   fullName,
   image,
   location,
   description,
   id,
 }
```
### reviews

```javascript
 {
   id,
   bookId,
   userName,
   bookTitle,
   comment,
   bookPages,
   progress,
 }
```

## Used API Endpoints in the App

| HTTP Method | URL                         | Request Body                 | Description                                                    |
| ----------- | --------------------------- | ---------------------------- | -------------------------------------------------------------- |
| GET         | `/books`                    |                              | Returns an array of all books                                                 |
| GET       | `/authors`                    |         | Returns an array of all authors                                             |
| GET         | `/books/:booksId`            |                     | Returns an object with the book details                                    |
| GET        | `/authors/:authorId`            |   | Returns an object with the author details                                            |
| POST      | `/authors`            | { fullName, location, description}      | Creates a new author object                                         |
| PUT        | `/books/:bookId`    `/authors/:authorId `             |    {title, author, image, published, pages,genre, serie,summary, rating, read, review}    | Updates all details of a single book                                              |
| PATCH        | `/books/:bookId`     `/authors/:authorId `             | {ratings}               | Updates rating property of a single book                                            |
| DELETE       | `/books/:bookId`                |               | Deletes a single book                                                 |
| GET      | `/authors/:authorId?_embed=books`            |                      | Returns a single author and all their books
 
## Links

### Collaborators

[Developer 1 name](https://github.com/NuriaSoley)

[Developer 2 name](https://github.com/Gemma-Fernandez)

### Project

[Repository Link Client](https://github.com/NuriaSoley/client-bookdragons-booshelves)

[Repository Link Server](https://github.com/Gemma-Fernandez/bookdragons-bookshelves/tree/master)

[Deploy Link](https://bookdragons-bookshelves.netlify.app/)


### Slides

[Slides Link](https://docs.google.com/presentation/d/1eXAty8IN5bckDhSq4J5fIyImB5t4WJw90FDAqiTkndI/edit#slide=id.g3084cdf60cb_0_60)