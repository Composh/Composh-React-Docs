Chip
Chips can be used to display entities in small blocks.


Flat chip
 
Outlined chip
 Usage
import * as React from 'react';
import { Chip } from 'react-native-paper';

const MyComponent = () => (
  <Chip icon="information" onPress={() => console.log('Pressed')}>Example Chip</Chip>
);

export default MyComponent;
Try this example on Snack 
Props
mode
Type: 'flat' | 'outlined'
Default value: 'flat'
Mode of the chip.

flat - flat chip without outline.
outlined - chip with an outline.
children (required)
Type: React.ReactNode
Text content of the Chip.

icon
Type: IconSource
Icon to display for the Chip. Both icon and avatar cannot be specified.

avatar
Type: React.ReactNode
Avatar to display for the Chip. Both icon and avatar cannot be specified.

selected
Type: boolean
Default value: false
Whether chip is selected.

selectedColor
Type: string
Whether to style the chip color as selected.

disabled
Type: boolean
Default value: false
Whether the chip is disabled. A disabled chip is greyed out and onPress is not called on touch.

accessibilityLabel
Type: string
Accessibility label for the chip. This is read by the screen reader when the user taps the chip.

onPress
Type: () => void
Function to execute on press.

onLongPress
Type: () => void
Function to execute on long press.

onClose
Type: () => void
Function to execute on close button press. The close button appears only when this prop is specified.

textStyle
Type: any
Style of chip's text

style
Type: StyleProp<ViewStyle>
theme
Type: Theme
testID
Type: string
Pass down testID from chip props to touchable for Detox tests.