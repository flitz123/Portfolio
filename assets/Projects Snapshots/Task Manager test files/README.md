# Task Manager Portfolio Evidence

## Project Overview

A responsive task management application built with a Go REST API and dependency-free frontend.

## SDLC Test Summary

### Frontend Development

- Verified initial dashboard and empty state
- Verified the create-task dialog and required task fields
- Verified task creation, editing, and completion
- Verified status filters and search
- Verified dark mode
- Verified mobile viewport layout at 390 x 844
- Confirmed test task cleanup returned the dashboard to a clean state

### Backend Development

- `GET /health` returned HTTP 200 with `{"status":"ok"}`
- `GET /tasks` returned the task collection
- `POST /tasks` created a task and returned HTTP 201
- `PUT /tasks/{id}` updated and completed the task
- `DELETE /tasks/{id}` removed the task successfully
- `go test ./...` passed for all packages

## Feature Screenshots

### Empty Dashboard

![Empty dashboard](screenshots/01-dashboard-empty.png)

### Task Creation

![Create task dialog](screenshots/02-create-task-dialog.png)

### Created Task

![Task created](screenshots/03-task-created.png)

### Completed Filter

![Completed task filter](screenshots/04-completed-filter.png)

### Search

![Task search](screenshots/05-search.png)

### Dark Mode

![Dark mode](screenshots/06-dark-mode.png)

### Mobile Layout

![Mobile layout](screenshots/07-mobile.png)

### Clean Final State

![Clean final dashboard](screenshots/08-clean-final.png)
