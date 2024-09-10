# Imagem
Tamanho original / Tamanho comprimido = Percentagem de compressão

número de linhas tem de ser múltiplo de 32

*nlex* -> número de linhas extra
*nlf* -> número de linhas falta
``nlex = nl % 32
``nlf = 32 - nlex

## Ver:
```python
numpy.repeat
numpy.vstack
numpy.hstack
??? dot || numpy.dot
```

## YCbCr
não utilizar formulas que estão no ppt
utilizar a matriz utilizando T = np.array(matriz) -> valores da matriz no ppt

decoder: não utilizar matriz no ppt
inverter T ultilizando Ti = np.linalg.inv(T)

fazer typecast
```python
R = Ti ... 
R = R.round().stype(np.uint8)
R = 255 -> 255.6 -> 256 -> 1
R [R < 0] = 0
R [R > 255] = 255
R = R.astype(np.uint8)
```

# Aula 2

## Ex6
Check `CV2.resize()` 
- utilizar `dzise` como `None`;
- testar `interpolation` como `INTER_LINEAR`, `INTER_AREA` e `INTER_CUBIC`;

4.2.0
- primeiro valor é sempre **4**;
- o segundo pode ser **1**, **2** ou **4**;
- o terceiro pode ser **0**, **1**, **2** ou **4**;
- se o terceiro for **0** existe compressão/downsampling *vertical*
## Ex7
Utilizar `scipy.fftpack.dct`

# Audio



