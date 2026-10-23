# Human-First Navigation (working title)

**Technology should adapt to people—not the other way around.**

An experimental, framework-independent approach to navigating mobile interfaces with minimal physical effort and fewer accidental activations. Originated while prototyping GreenMonster, but intentionally developed for use by anyone.

## Run the prototype

Open [`index.html`](index.html) in a browser. No build tools, accounts, database, external libraries, microphone, camera, or GPS required.

## Current experiment

- Follow a comfortable diagonal thumb arc; right/left-handed modes.
- Smooth 3D four-face rotating cube previews menu subjects.
- Lift thumb to stop; enlarged preview appears automatically.
- ENTER confirms explicitly; arrows offer an alternate path.
- Five example sections with contextual feature menus.

**Status:** Early usability prototype, not a production-ready accessibility component. The 6-inch radius is a design reference only, not a calibrated physical measurement. The demo does not contain working back-end functions, nor has it been validated for assistive technology or broad handset support.

## Principles

1. Human comfort over convention.
2. One contextual menu at a time, uncluttered screen.
3. Minimal actions between intent and result.
4. Distinguish preview from activation.
5. Provide equivalent controls for people who cannot swipe.
6. Privacy by default: no microphone, camera or GPS without explicit permission.
7. Measure comfort, errors, effort and speed with real users before claiming improvement.

## Roadmap

1. Document and stabilize gesture, selection and confirmation behavior.
2. Extract a standalone menu state engine from the GreenMonster demo.
3. Make cube visualization an optional adapter, not a required dependency.
4. Add keyboard, screen-reader and switch-access testing; confirm reduced-motion mode.
5. Calibrate each user's comfortable start/end thumb positions and motion path.
6. Add a voice-command adapter that uses the same menu events, only with explicit microphone opt-in.
7. Compare real-task efficiency with conventional interfaces.

## Project separation

The navigation component should contain no GreenMonster-specific business logic. GreenMonster will be a consumer of the component and a real-world test environment.

## License

This project is released under the MIT License.

See the [LICENSE](LICENSE) file for details.

## Contributing

See [`CONTRIBUTING.md`](CONTRIBUTING.md).
