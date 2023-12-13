# nobu10_data_bgm_format
蒼天録 - データ - BGM - フォーマット

蒼天録のBGMフォルダにある BGM/BGM**.NBX は全てフォーマットはただの WMA(Windows Media Audio) である。  
ffmpeg などで WMV もしくは WMA として変換して、拡張子だけ .NBX とすれば再生できる

.WMV や .WMV への変換は各種ツールや ffmpeg で行える。

`cmd
ffmpeg -i input.m4a -acodec wmav2 -b:a 320k output.wma
`