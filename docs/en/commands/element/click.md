# Click

Click element at its center point.
## Example Usage

```java
// Java
MobileElement el = driver.findElementByAccessibilityId("SomeId");
el.click();

```
```python
# Python
el = self.driver.find_element_by_accessibility_id('SomeId')
el.click();

```
```javascript
// Javascript
// webdriver.io example
driver.click('#SomeId');


// wd example
let element = await driver.elementByAccessibilityId('id', 'SomeId');
await element.click();

```
```ruby
# Ruby
@driver.find_element(:accessibility_id, 'SomeId').click

```
```php
# PHP
// TODO

```
```csharp
// C#
// TODO

```

## Description

Clicks element at its center point. If the element's center point is obscured by another element, an element click intercepted error is returned. If the element is outside the viewport, an element not interactable error is returned.
Not all drivers automatically scroll the element into view and may need to be scrolled to in order to interact with it.


## Client Docs

* [Java](https://seleniumhq.github.io/selenium/docs/api/java/org/openqa/selenium/WebElement.html#click--)
* [Python](http://selenium-python.readthedocs.io/api.html#selenium.webdriver.remote.webelement.WebElement.click)
* [Javascript (WebdriverIO)](http://webdriver.io/api/action/click.html)
* [Javascript (WD)](https://github.com/admc/wd/blob/master/lib/commands.js#L1672)
* [Ruby](http://www.rubydoc.info/gems/selenium-webdriver/Selenium/WebDriver/Element#click-instance_method)
* [PHP](https://github.com/appium/php-client/)
* [C#](https://github.com/appium/appium-dotnet-driver/)

## Support

### Appium Server

|Platform|Driver|Platform Versions|Appium Version|Driver Version|
|--------|----------------|------|--------------|--------------|
| iOS | [XCUITest](/docs/en/drivers/ios-xcuitest.md) | 9.3+ | 1.6.0+ | All |
|  | [UIAutomation](/docs/en/drivers/ios-uiautomation.md) | 8.0 to 9.3 | All | All |
| Android | [UiAutomator2](/docs/en/drivers/android-uiautomator2.md) | ?+ | 1.6.0+ | All |
|  | [UiAutomator](/docs/en/drivers/android-uiautomator.md) | 4.2+ | All | All |
| Mac | [Mac](/docs/en/drivers/mac.md) | ?+ | 1.6.4+ | All |
| Windows | [Windows](/docs/en/drivers/windows.md) | 10+ | 1.6.0+ | All |

### Appium Clients 

|Language|Support|
|--------|-------|
|[Java](https://github.com/appium/java-client/releases/latest)| All |
|[Python](https://github.com/appium/python-client/releases/latest)| All |
|[Javascript (WebdriverIO)](http://webdriver.io/index.html)| All |
|[Javascript (WD)](https://github.com/admc/wd/releases/latest)| All |
|[Ruby](https://github.com/appium/ruby_lib/releases/latest)| All |
|[PHP](https://github.com/appium/php-client/releases/latest)| All |
|[C#](https://github.com/appium/appium-dotnet-driver/releases/latest)| All |

## HTTP API Specifications

### Endpoint

`POST /wd/hub/session/:session_id/element/:element_id/click`

### URL Parameters

None

### JSON Parameters

None

### Response

null

## See Also

* [W3C Specification](https://www.w3.org/TR/webdriver/#element-click)
* [JSONWP Specification](https://github.com/SeleniumHQ/selenium/wiki/JsonWireProtocol#sessionsessionidelementidclick)
