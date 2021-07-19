<p align="center" >
  <img src="https://github.com/JanyGee/JGOCTimer/blob/main/Source/icon.png">
</p>

# JGOCTimer
[![Version](https://img.shields.io/cocoapods/v/JGOCTimer.svg?style=flat)](http://cocoapods.org/pods/JGOCTimer)
[![License](https://img.shields.io/cocoapods/l/JGOCTimer.svg?style=flat)](http://cocoapods.org/pods/JGOCTimer)
[![Platform](https://img.shields.io/cocoapods/p/JGOCTimer.svg?style=flat)](http://cocoapods.org/pods/JGOCTimer)
[![Swift-5.0](http://img.shields.io/badge/Swift-5.0-blue.svg)]()

JGOCTimer is a lightweight timer extension for OC.

## Installation

JGOCTimer is available through [CocoaPods](http://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod "JGOCTimer"
```

## Usage

```OC
#import "JGTimer.h"
```

## Methods
** (NSString *)executeTask:(void (^)(void))task start:(NSTimeInterval)start interval:(NSTimeInterval)interval repeats:(BOOL)repeats async:(BOOL)async**
```OC
[JGTimer execTask:self selector:@selector(doTask) start:2.0 interval:1.0 repeats:YES async:NO];
```

** (NSString *)executeTask:(id)target selector:(SEL)selector start:(NSTimeInterval)start interval:(NSTimeInterval)interval repeats:(BOOL)repeats async:(BOOL)async**
```OC
[JGTimer executeTask:^{[self doTask];} start:2.0 interval:1.0 repeats:YES async:NO];
```
