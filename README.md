### VibratorService使用简介

```
Vibrator vibrator = (Vibrator) getSystemService(Context.VIBRATOR_SERVICE);
Toast.makeText(this, "手机震动", Toast.LENGTH_LONG).show();
vibrator.vibrate(3000);
vibrator.cancel();
long[] vib = new long[]{400, 800, 1200, 1800};
vibrator.vibrate(vib, 2);//2  指的是，从数组 vib 中的索引位置开始循环震动
```
