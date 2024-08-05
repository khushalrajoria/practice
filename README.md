# CSS and JS Animations and Transitions Practice

This repository contains my practice work for implementing various CSS and JavaScript animations and transitions. The focus is on creating smooth, interactive user interfaces using modern web development techniques.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Features

- Smooth background color transitions
- Inline list items with hover effects
- Video container with overlay effects
- Interactive image scaling and transitions
- Keyframe animations for rotating and resizing images

## Installation

1. Clone the repository:

```bash
git clone https://github.com/your-username/css-js-animations-practice.git
```

2. Navigate to the project directory:

```bash
cd css-js-animations-practice
```

## Usage

Open `index.html` in your preferred web browser to view the animations and transitions in action.

## Code Overview

### CSS

- **Background Color Transition:**

```css
body {
    background-color: #121212;
}
```

- **Inline List Items with Hover Effects:**

```css
ul li {
    display: inline;
    margin-left: 6px;
}

ul li a {
    color: aliceblue;
    padding: 7px;
    padding-left: 19px;
    padding-right: 19px;
    border-radius: 5px;
}

ul li a:hover {
    color: black;
    background-color: aliceblue;
    transition-timing-function: ease-in-out;
    transition-duration: .31s;
}
```

- **Video Container with Overlay Effects:**

```css
.video-container {
    height: 490px;
    width: 100%;
    position: relative;
}

.video-container video {
    width: 100%;
    height: 100%;
    position: absolute;
    object-fit: cover;
    z-index: 0;
    opacity: 30%;
}

.video-container video:hover {
    opacity: 100%;
    transition-duration: .9s;
}
```

- **Interactive Image Scaling and Transitions:**

```css
.loid img:hover,
#yor img:hover {
    transform: scale(1.1);
    transition-timing-function: ease-in-out;
    transition-duration: .4s;
}
```

- **Keyframe Animations for Rotating and Resizing Images:**

```css
@keyframes changeSize {
    0% {
        width: 100%;
        height: 100%;
    }
    70% {
        width: 70%;
        height: 70%;
    }
    100% {
        width: 1%;
        height: 1%;
    }
}

@keyframes rotate {
    0% {
        transform: rotate(0deg);
    }
    10% {
        transform: rotate(0deg);
    }
    100% {
        transform: rotate(360deg);
    }
}

#testcase:hover > img {
    animation-name: rotate, changeSize;
    animation-delay: .8s;
    animation-duration: 1s, 1s;
    animation-iteration-count: 1, 1;
    animation-direction: alternate, alternate;
}
```

## Contributing

Contributions are welcome! Feel free to submit a pull request or open an issue to discuss improvements, bug fixes, or new features.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
