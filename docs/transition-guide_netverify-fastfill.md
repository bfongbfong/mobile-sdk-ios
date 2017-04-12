![Fastfill & Netverify](images/netverify.png)

# Transition guide for Fastfill & Netverify Mobile

## 2.5.0

#### Changes in visual customization
Removed _NetverifyCameraFlashButton_ as the icons to switch camera and toggle flash were moved to the navigation bar.

#### Changes in Localizable-Netverify.strings
Multiple additions and changes in regards to the new guidance / help screen.

## 2.4.0
No backward incompatible changes.

## 2.3.1
No backward incompatible changes.

## 2.3.0
#### Renamed enum types
Renamed the following enum types:
 * `NVDocumentVariant` to `NetverifyDocumentVariant`
 * `NVGender` to `NetverifyGender`
 * `NVMRZFormat` to `NetverifyMRZFormat`
 * `NVExtractionMethod` to `NetverifyExtractionMethod`.

#### Removed name match feature
Name matching by comparing a provided name with the extracted name from a document was removed. The property _name_ in NetswipeViewController class is deleted, as well as the boolean _nameMatch_ and integer _nameDistance_ in NetswipeCardInformation class.

## 2.2.0
#### Removed liveness detection result
Parameter `livenessDetected` has been removed from `NetverifyDocumentData`.

## 2.1.0
#### Exceptions at initialisation
An exception is thrown in case mandatory parameters in the `NetverifyConfiguration` object are invalid.

#### Changes in Localizable-Netverify.strings
Removed one string in regards to scanning not possible.