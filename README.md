# SURGE Web Control

Static browser prototype for a robot-control interface with an on-screen joystick, speed control and gamepad input.

## Current status

The application is contained in `index.html`. The gamepad loop calculates left and right wheel speeds and writes them to the browser console. Robot transport is a placeholder: this branch does not send those values to a JetBot or another device, and it does not implement live device telemetry.

## Preview

```sh
python3 -m http.server 8080
```

Open `http://localhost:8080` and connect a browser-compatible gamepad to exercise the input handling. External font and icon resources require a network connection.

There is no `package.json`, npm install step or npm start script in this repository. Browser/gamepad support and a real transport adapter should be tested before connecting hardware.

## License

See [LICENSE](LICENSE), which contains the GNU GPL version 3 text.
