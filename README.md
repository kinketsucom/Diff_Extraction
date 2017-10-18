# メモ
## numpyでのuint8の引き算(今はこうしか思いつかないが)

```python
#配列1,bの引き算をする
a = np.uint8([1,3])
b = np.uint8([2,2])
#intにキャスト
a = a.astype(int)
b = b.astype(int)
#intとして引き算して、絶対値を取る
c = a - b
c = abs(c)
#uint8にキャストして戻す
c = np.uint8(c)
```
