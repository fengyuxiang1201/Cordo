# Cordo
使用react-native开发混合app。

## swiper的使用

### 使用地址
https://github.com/leecade/react-native-swiper

###安装
```bash
$ npm i react-native-swiper --save
```
### 使用demo的部分代码
```jsx
class Slider extends Component {
  _onTouchEnd(e, state, context) {
    if(state.total == (state.index + 1)){
        alert('去登录');
    }
  }
  render() {
    return (
     <Swiper showsButtons={false} loop={true} onMomentumScrollEnd={this._onTouchEnd}>
        <Image style={styles.img} source={{uri: sliderImgs[0]}}></Image>
        <Image style={styles.img} source={{uri: sliderImgs[1]}}></Image>
        <Image style={styles.img} source={{uri: sliderImgs[2]}}></Image>
      </Swiper>
    )
  }
}
```
