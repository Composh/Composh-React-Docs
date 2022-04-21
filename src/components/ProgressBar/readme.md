ProgressBar
Progress bar is an indicator used to present progress of some activity in the app.


 Usage
import * as React from 'react';
import { ProgressBar, Colors } from 'react-native-paper';

const MyComponent = () => (
  <ProgressBar progress={0.5} color={Colors.red800} />
);

export default MyComponent;
Try this example on Snack 
Props
progress
Type: number
Default value: 0
Progress value (between 0 and 1).

color
Type: string
Color of the progress bar. The background color will be calculated based on this but you can change it by passing backgroundColor to style prop.

indeterminate
Type: boolean
If the progress bar will show indeterminate progress.

visible
Type: boolean
Default value: true
Whether to show the ProgressBar (true, the default) or hide it (false).

style
Type: StyleProp<ViewStyle>
theme
Type: ReactNativePaper.Theme