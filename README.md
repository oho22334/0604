# 0604
# 聲音
```C
import processing.sound.*;
SoundFile player;///用sound外掛發出聲音
void setup(){
  size(400,200);
  player = new SoundFile(this, "bell.mp3" );///放入bell鈴聲
}
void draw(){
  background(51,114,191);///背景顏色
}
void mousePressed(){
  if(player.isPlaying()){///讓他點一下能停止或開始
    player.stop();
  }else{
  player.play();
}
}
```
