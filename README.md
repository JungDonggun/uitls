# utils

```c
export const newArray(index: numer) => {
  return new Array(index).fill('_').map(() => '')
}

export const emailCheck = (email: string) => {
  const emailCheck = /^[A-Za-z0-9_.-]+@[A-Za-z0-9-]+.[A-Za-z0-9-]+/
  if (emailCheck.test(email) === false) {
    Alert.alert('이 메일형식이 올바르지 않습니다.')
    return false
  }
  // alert('이메일 형식만 체크됩니다.')
  return true
}


export const numberFormat = (inputNumber: string) => inputNumber.toString().replace(/\B(?=(\d{3})+(?!\d))/g, ',')


export const replaceComma = (pStr: string) => {
  const strCheck = /\,/g
  pStr = pStr.replace(strCheck, '')
  return pStr
}

```
