# Overview

The pipelines course will cover how to use the pipelines pattern in python to build production-grade ETL pipelines using pandas, pandera, and dataclasses.

# Content

## Lesson 1

- Example of how a functional pipeline looks like (Use a sample data set, load it in pandas, perform some transformations, and print the head).
- Go over the weaknesses of this pattern, such as testability (no way to mock input/output), runtime exceptions (defects in the data that could cause a runtime failure), and lack of type checking.
- Quick (5 slide) demo of how the pipelines pattern works, how pandera works, and how tools like ruff and mypy work with it.
- Perform in-line update to implement the updates, and show ruff and mypy in work.

## Lesson 2

- Update pipeline to use a class
- Explain how the class allows polymorphism with the pipelines to simplify their execution
- Introduce logging with the pipelines
- Introduce using async to call the pipelines for parallel processing

## Lesson 3

- Introduce pipeline factory for building pipelines
- Use pipeline factory to build endpoints (Tool Call, Fastapi, MCP)

## Lesson 4

- Connect endpoints to frontend (streamlit, chainlit + tool call, MCP + openwebui)

## Lesson 5

- storing the data in a locally hosted databae
- Host postgresql db
- Build ORM and engine in sql alchemy
- Store data in postgresql db