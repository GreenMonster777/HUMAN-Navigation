# Interaction specification (draft)

The arc and cube are separate concerns:

- **Input:** pointer gesture along a comfortable arc; arrow/keyboard and future voice alternatives.
- **Navigation state:** current level, focused item, provisional swipe position, selected item.
- **Display:** rotating 3D illusion that previews items; only current content needs to be interactive.
- **Release:** stop input and enlarge/readably preview focused item; do not activate it.
- **Confirm:** explicitly press ENTER to open the item.
- **Correction:** arrows shift the focus without requiring a new swipe.
- **Handedness:** mirror touch geometry, not information hierarchy or safety rules.
- **Safety:** destructive or emergency actions must need deliberate confirmation.

Future API should expose events such as `preview`, `focus`, `confirm`, and `back`. Avoid tying application navigation to cube-specific transforms. Navigation should preserve browser history and page accessibility.

## Known limitations of the current demo

- The curved track uses illustrative control points, not physical inches.
- The prototype is not yet calibrated to the person's thumb path.
- Real-phone usability and screen-reader testing remain outstanding.
- Visual motion and responsiveness will need auditing across devices.
