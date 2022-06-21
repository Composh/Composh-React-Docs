To use the hook, App.js

import useLongPress from "./useLongPress";

export default function App() {

    const onLongPress = () => {
        console.log('longpress is triggered');
    };

    const onClick = () => {
        console.log('click is triggered')
    }

    const defaultOptions = {
        shouldPreventDefault: true,
        delay: 500,
    };
    const longPressEvent = useLongPress(onLongPress, onClick, defaultOptions);

    return (
        <div className="App">
            <button {...longPressEvent}>use  Loooong  Press</button>
        </div>
    );
}