# Gold Runner

## Background

Gold Runner was a game written for the Tandy Color Computer in 1984. It bears a striking resemblance to a game called Lode Runner for the Apple 2 and other 8 bit computers of the time.

In 1997 I wrote a clone of Gold Runner for a hobbyist computer called the MM/1. This computer was something of a descendant of the Tandy Color Computer 3, and a number of people from the Color Computer (CoCo) community migrated there once the mainstream computing world had moved onto 16 bit systems.

In 2008 I resurrected the code from the MM/1 version and ported it to the iPhone and released it to the App Store.

Within a year, a company that had bought the rights to the original Lode Runner property began seeking out games on various platforms that they believed infringed on their newly acquired intellectual property. A number of games, including Gold Runner for iOS, were targeted and removed from sale.

It has long been my intention to modify the game engine such that it could no longer be considered derivative of their intellectual property, but I've never gotten around to it. Now I think it best to just release the project in its entirety to the public so that anyone who was a fan of Gold Runner can play and extend it.

While the app was available for sale, it had one major complaint, the control scheme. There is no perfect scheme for controlling a tiny character on a touch screen, but I provided three methods: 1) on-screen buttons where the character only moves as you're touching the button 2) on-screen buttons where touching a button starts the character in motion until a different button is pushed 3) flicking the screen in a direction starts the character moving in that direction until another flick is performed or the screen is tapped. I would be greatly interested in seeing what better control schemes people could come up with.

The original codebase was written in 'C' on a system that didn't have what would be considered frameworks or even a reasonable set of APIs by modern standards. It was shoehorned into classes to fit iOS design patterns. As such, it isn't exactly the most sparkling set of code I've ever written, not to mention the fact that I wrote the original code just two years into my professional programming career, some 15 years ago. Nevertheless, it works, and shouldn't be too difficult to understand.

## History

Version 1.0:	Initial release

## Classes

Classic_Gold_RunnerAppDelegate

This is the application delegate. It performs all game setup functions and manages flow of the game and the buttons and high score display of the primary screen. Most of the game code is in this class.

Classic_Gold_RunnerViewController

This class manages user input and player control.

Character

This class manages character movement, path checking for character movement and search patterns for the guards.

FlickView

This class manages input for the overlay view that processes user flicks when using the flick control scheme.

Gameboard

This class manages the game boards that define each level.

ImageSet

This class manages parsing sprites from the file format used by the assets from the original MM/1 version.

Palette

This class manages parsing the color palette from the file format used by the assets from the original MM/1 version.

RawImage

This class manages parsing an individual image from the file format used by the assets from the original MM/1 version.

## Support

Questions, suggestions or contributions to the codebase can be submitted to support@infusionsofgrandeur.com

## License

Copyright 2008 Infusions of Grandeur

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
