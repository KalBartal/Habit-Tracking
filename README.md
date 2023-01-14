# README.md
# # Habit Tracking

This is my coding challenge submission for day #37 of the 100 Days of Code: The Complete Python Pro Bootcamp, instructor-led training

This Python app provides a simple interface to make requests to Pixela, a graph data service. With this app, you can POST a new user account, POST a new graph, POST data for a new pixel, PUT updates for a pixel, and DELETE a pixel.

## Requirements
- Python 3+
- Requests (`pip install requests`)

## Configuration
Before you can make requests to Pixela, you'll need to enter your credentials in the code: 
```
USERNAME = "YOUR USERNAME"
TOKEN = "YOUR SELF GENERATED TOKEN"
GRAPH_ID = "YOUR GRAPH ID"
```

## Usage
To use this app, just uncomment the appropriate code block:
- POST a new user account: 
```
response = requests.post(url=pixela_endpoint, json=user_params)
```

- POST a new graph: 
```
response = requests.post(url=graph_endpoint, json=graph_config, headers=headers)
```

- POST data for a new pixel: 
```
response = requests.post(url=pixel_creation_endpoint, json=pixel_data, headers=headers)
```

- PUT updates for a pixel: 
```
response = requests.put(url=update_endpoint, json=new_pixel_data, headers=headers)
```

- DELETE a pixel: 
```
response = requests.delete(url=delete_endpoint, headers=headers)
```

[//]: # (## License)

[//]: # (This project is licensed under the MIT License.)