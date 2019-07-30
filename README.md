# react-native-box-shadow

[boxShadow]

- x: offsetX
- y: offsetY
- offset: {x, y}
- blur: blurRadius
- spread: spreadRadius
- color
- inset

```javascript
import BoxShadow from 'react-native-box-shadow';

/* offset-x | offset-y | color */
// box-shadow: 60px -16px teal;
<BoxShadow x={60} y={-16} color="teal" />;

/* offset-x | offset-y | blur-radius | color */
// box-shadow: 10px 5px 5px black;
<BoxShadow x={10} y={5} blur={5} color="black" />;

/* offset-x | offset-y | blur-radius | spread-radius | color */
// box-shadow: 2px 2px 2px 1px rgba(0, 0, 0, 0.2);
<BoxShadow x={2} y={2} blur={2} spread={1} color="rgba(0, 0, 0, 0.2)" />;

/* inset | offset-x | offset-y | color */
// box-shadow: inset 5px 1px gold;
<BoxShadow inset x={5} y={1} color="gold" />;

/* Any number of shadows, separated by commas */
// box-shadow: 3px 3px red, -1em 0 0.4em olive;

<BoxShadow
  shadows={[
    { x: 3, y: 3, color: 'red' },
    { x: -1, y: 0, blur: 0.4, color: 'olive' }
  ]}
/>;
```

### License

MIT
