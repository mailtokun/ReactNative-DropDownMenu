
# react-native-dropdownmenus

<img height="530" width="300" src="https://raw.githubusercontent.com/pengweiqiang/ReactNative-DropDownMenu/master/screenShot/demo.png"  align=center />

## Getting started

`$ npm install react-native-dropdownmenus --save`

### Mostly automatic installation

`$ react-native link react-native-dropdownmenus`


## Usage
```javascript
import DropdownMenu from 'react-native-dropdownmenus';

let conditionData = [["one", "tow", "three"], ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"],
                        ["Java", "PHP", "C#", "JS", "C++", "Python"]];
<DropdownMenu
                style={{flex: 1}}
                bgColor={'white'}
                tintColor={'#666666'}
                activityTintColor={'green'}
                resetRight={true} // 联动，将右侧所有的下拉框的index重置为0
                // arrowImg={}
                // checkImage={}
                // optionTextStyle={{color: '#333333'}}
                // titleStyle={{color: '#333333'}}
                maxHeight={300}
                handler={(selection, row) =>
                    console.log(selection,row)
                }
                data={conditionData}
                selectIndex={[0,2,0]}>
                
</DropdownMenu>
```
### Param
| Parameter | Type | Default | Description
| ------ | ------ | ------ | ------ |
| bgColor | string |  | backgroud color
| tintColor | string |  | normal text color
| activityTintColor | string |  | active text color 
| maxHeight | number |  | max Height
| hanlder | func |  | selected item onclickListener
| data | Array |  | show Data
| selectIndex | string |  | default selected index




