# Laravel API

This repository contains the documentation for the Laravel API.

## API Endpoints

### All Tasks

- Method: GET
- URL: `http://127.0.0.1:8000/api/v1/tasks`

#### Retrieve A Single Task

- Method: GET
- URL: `http://127.0.0.1:8000/api/v1/tasks/{task_id}`

#### Store Task

- Method: POST
- URL: `http://127.0.0.1:8000/api/v1/tasks`
- Headers:
  - Accept: application/json
- Body:
  ```json
  {
      "name": "This is Jay's Task"
  }
#### Update Task
-Method: PUT
-URL: http://127.0.0.1:8000/api/v1/tasks/{task_id}
-Headers:
 -Accept: application/jsonBody:
 - Body:
  ```json
    {
        "name": "Task One Updated"
    }

#### Change Task Status
-Method: PATCH
-URL: http://127.0.0.1:8000/api/v1/tasks/{task_id}/complete
-Headers:
 -Accept: application/json
  -Body:
  ```json
    {
        "is_completed": true
    }


#### Delete Task
-Method: DELETE
-URL: http://127.0.0.1:8000/api/v1/tasks/{task_id}
 -Headers:
  -Accept: application/json
