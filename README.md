# FastAPI05

This is intended to show examples of using FastAPI and asyncio.

In the short run, it will show examples of using the Item model in SQLAlchemy.

Perhaps it should show an example of SQLAlchemy 2.x.

## Setup database

Name is "fastapi05"

```
create database fastapi05;
```

One table for items.

Add some records like:

```
insert into items (name, description,price, created_at, updated_at)
values ("Zealot", "Protoss action figure", 66, current_timestamp(), current_timestamp());
```

## Running this

To run it:

```
cd src
uvicorn main:app --reload
```

Then send HTTP requests to localhost:8000, such as:

http://localhost:8000/

http://localhost:8000/items

http://localhost:8000/items/2
