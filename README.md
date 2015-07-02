# Gradientify

A simple jQuery plugin that provides CSS gradient transitions.

Based on the script by Mike Byrne:

http://opticalcortex.com/animating-css-gradients/

## Usage

Here is an example of quick usage:

```php
$('body').gradientify({
    gradients: [
        { start: [49,76,172], stop: [242,159,191] },
        { start: [255,103,69], stop: [240,154,241] },
        { start: [33,229,241], stop: [235,236,117] }
    ]
});
```

### Parameters:

Name | Description | Required? | Default 
---- | ----------- | -------- | -------
gradients | An array of objects containing start and stop gradients in RGB values. | **required** | []
angle | The gradient angle. The value is put directly in the CSS gradient definition. | optional | 0deg
fps | Frames per second. The higher the value the transition will be smoother, but it affects the performance! | optional | 60
transition_time | Transition time between gradients in seconds. | optional | 8