---
layout: post
title: My Collection Database
subtitle: For Building a Gaming List
cover-img: /assets/img/background2jpg
thumbnail-img: /assets/img/databasethumbnail.jpg
share-img: /assets/img/background2.jpg
gh-repo: daattali/beautiful-jekyll
tags: [game, collection, database, list, gaming list]
comments: true

---
**Goals**
- Allow users to save a list of their favorite games
- Rating for games can be updated
- Games can be deleted from the collection

**Potential Features**
- Creating a format for the database
- Adding buttons to place games from search bar to My Collection Database

### Updates

{: .box-note}
**01/13/22:** Database Basics Created

My Collection Frontend:

![Collection](/assets/img/mycollection.png)

Sample Code for Database:

```javascript
<tr th:each="person : ${list}">
    <td th:text="${person.teacher_class}" >Game</td>
    <td th:text="${person.rating}" >Rating</td>

    <td style="color:Black;" >
        <a th:href="@{/Database/personupdate/{id}(id = ${person.id})}">Update</a>
        <a th:href="@{/Database/persondelete/{id}(id = ${person.id})}">Delete</a>
    </td>
</tr>
```