# API documentation

GET - all tasks
- https://mockend.com/mockend/demo/posts
```
 {
    "createdAt": "2022-09-05T17:40:20Z",
    "id": 98,
    "priority": 1,
    "state": "incomplete",
    "title": "perspiciatis at"
 },
 {
    "createdAt": "2022-09-03T22:23:30Z",
    "id": 99,
    "priority": 10,
    "state": "incomplete",
    "title": "consequuntur ducimus alias"
 },
```

GET - task by ID
- https://mockend.com/mockend/demo/posts/1

```
 {
    "createdAt": "2022-09-03T22:23:30Z",
    "id": 1,
    "priority": 10,
    "state": "incomplete",
    "title": "consequuntur ducimus alias"
 }
```

GET - sort tasks (priority)
> priority 100 represents very important  
> priority 10 represents important  
> priority 1 represents not important
- https://mockend.com/mockend/demo/posts?priority_eq= [100 | 10 | 1]

```
 {
    "createdAt": "2022-09-05T17:40:20Z",
    "id": 98,
    "priority": 100,
    "state": "complete",
    "title": "perspiciatis at"
 },
 {
    "createdAt": "2022-09-03T22:23:30Z",
    "id": 99,
    "priority": 100,
    "state": "incomplete",
    "title": "consequuntur ducimus alias"
 },
```

GET - sort tasks (state)
- https://mockend.com/mockend/demo/posts?state_eq= [completed | incomplete]
```
 {
    "createdAt": "2022-09-05T17:40:20Z",
    "id": 98,
    "priority": 10,
    "state": "incomplete",
    "title": "perspiciatis at"
 },
 {
    "createdAt": "2022-09-03T22:23:30Z",
    "id": 99,
    "priority": 100,
    "state": "incomplete",
    "title": "consequuntur ducimus alias"
 },
```