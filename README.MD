# Happy Birthday Android App

This Android Studio project is a simple birthday greeting app that displays a birthday message along with an image. It utilizes Jetpack Compose for building the user interface.

## Features

- Displays a birthday greeting message with an accompanying "from" message.
- Includes an image for added visual appeal.

## Prerequisites

- Android Studio (version Flamingo | 2022.2.1 or higher)

## Getting Started

1. Clone the repository or download the source code.
2. Open the project in Android Studio.
3. Build and run the app on an emulator or a physical device.

## Usage

1. Launch the app on your Android device or emulator.
2. The app will display a birthday greeting with an image and a "from" message.
3. Customize the birthday message and the "from" message by modifying the message and from parameters in the MainActivity class.

```
Surface(
modifier = Modifier.fillMaxSize(),
color = MaterialTheme.colorScheme.background
) {
BirthdayGreetingWithImage("Happy Birthday Sam!", "- from Emma")
}
```

4. You can also modify the styling of the birthday message and the "from" message by adjusting the font size in the BirthdayGreetingWithText function.

```
@Composable
fun BirthdayGreetingWithText(message: String, from: String, modifier: Modifier = Modifier) {
    Column(modifier = modifier) {
        Text(
            text = message,
            fontSize = 36.sp
        )
        Text(
            text = from,
            fontSize = 24.sp
        )
    }
}
```

## Preview

A preview of the birthday card can be viewed using the BirthdayCardPreview function.

```
@Preview(showBackground = true)
@Composable
fun BirthdayCardPreview() {
    HappyBirthdayTheme {
        BirthdayGreetingWithImage("Happy Birthday Sam!", "- from Emma")
    }
}
```

## Dependencies

This project relies on the following dependencies:

- android.os.Bundle
- androidx.activity.ComponentActivity
- androidx.activity.compose.setContent
- androidx.compose.foundation.Image
- androidx.compose.foundation.layout.Box
- androidx.compose.foundation.layout.Column
- androidx.compose.foundation.layout.fillMaxSize
- androidx.compose.material3.MaterialTheme
- androidx.compose.material3.Surface
- androidx.compose.material3.Text
- androidx.compose.runtime.Composable
- androidx.compose.ui.Modifier
- androidx.compose.ui.res.painterResource
- androidx.compose.ui.tooling.preview.Preview
- androidx.compose.ui.unit.sp

## License

This project is licensed under the MIT License. Feel free to use, modify, and distribute the code as needed.
