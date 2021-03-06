# VPRangeSlider
This is a 2 way slider for iOS. You can create segmented or
unsegmented range sliders. Similar to price range selector
seen in different apps/websites. You can customize the views as
per your requirements.

## Installation
Drag and drop the VPRangeSlider.h and VPRangeSlider.m into project file

## Requirements

1. iOS 7.0 or later.
2. ARC memory management.

## Usage
After adding VPRangeSlider.h and VPRangeSlider.m files into your project, there are 2 ways to create slider.

1. By adding an empty view to your xib/storyboard and 
changing the class of the view to VPRangeSlider. After adding the view
create an outlet.

2. Programmatically set the property for the view.

For the oulet/property of the view set the necessary properties. 
If more customization is needed, you can set the optional parameters.

If the requiresSegments is set to YES, then segmented range slider is created. Else normal slider is created.

If needed, then you can make use of 2 delegates.

- (void)sliderScrollingWithMinPercent:(CGFloat)minPercent andMaxPercent:(CGFloat)maxPercent

This delegate is called every time the slider is moved/panned until the sliding stops.

- (void)sliderScrolledToMinIndex:(NSInteger)minIndex andMaxIndex:(NSInteger)maxIndex
This delegate is called when the slider stops at any segmented index.

# ![Screenshot](/VPRangeSlider-Screenshot.png)

## Contributing
1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## History
Version 0.1.0

Basic slider with all the necessary functions like 2 way slider with/without 
segments and properties for handling different views and colors.

## License
The MIT License (MIT)

Copyright (c) 2015 Varun P M

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
