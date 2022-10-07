# React Deadline

Countdown Timer for React and React Native

## Install
`npm install react-deadline --save`

```
import CountdownTimer from 'react-deadline';

...

render() {
  return (
    <CountdownTimer
      endsAt={this.props.date}
      onUpdate={timer => this.setState({timer: timer})>
      {`${this.state.timer.hours}:${this.state.timer.minutes}:${this.state.timer.seconds}`}
    </CountdownTimer>
  )
}
```

## Properties

- `endsAt` __string__ - any string that [moment js](http://momentjs.com/) can parse
- `onUpdate` __function__ - called every 1000ms (1 second). Use this to set your state to the timer values.

## Dependencies
- [react timer mixin](https://github.com/reactjs/react-timer-mixin)
- [moment.js](http://momentjs.com)
