# GMCamera
Small and easy to use camera system for GameMaker.

### Basic setup.
- Create a script in GameMaker.
- Copy everything from GMCamera.gml.
- Paste to script file.
- Create a persistent object named `obj_camera_controller` for example, and add it to init/starting room.
- Add to create event:
```gml
camera = new GMCamera(_game_width, _game_height); //Change to desired values.
camera.size(_width, _height);                     //Change to desired values.
camera.target(_instance);                         //Change to desired target. Hover for info.
camera.enable();
```
- Add to end step event:
```gml
camera.update();
```
- And you are set to go.
