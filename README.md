# uitls

```c
export const emailCheck = (email: string) => {
  const emailCheck = /^[A-Za-z0-9_.-]+@[A-Za-z0-9-]+.[A-Za-z0-9-]+/;
  if (emailCheck.test(email) === false) {
    Alert.alert('이 메일형식이 올바르지 않습니다.');
    return false;
  }
  // alert('이메일 형식만 체크됩니다.');
  return true;
};


export const numberFormat = (inputNumber: string) => {
  return inputNumber.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ',');
};


export const replaceComma = (pStr: string) => {
  var strCheck = /\,/g;
  pStr = pStr.replace(strCheck, '');
  return pStr;
};
```
