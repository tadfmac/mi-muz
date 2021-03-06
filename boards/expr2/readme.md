# mi:muz:expr#2 ATtiny841 Hybrid MIDI Test Board 

ATtiny841用のHybrid MIDI Test Boardです。
専用のファームウエア[HybridMidiATtiny](https://github.com/tadfmac/mi-muz/tree/master/arduino/libraries/HybridMidiAttiny)を利用することで、
USBに刺せばUSB MIDIデバイス、mi:muz:mstrシールドと組み合わせれば、I2C MIDIデバイスとして利用することができます。

![mi:muz:expr#2](./mimuz-expr2-image.png)

# Version

v0.22 (2015.07.05)

# Schematics

![mimuz-expr2-v021.png](./mimuz-expr2-v021.png)

## parts

- U1:ATtiny841-SSU
- JP1:ピンヘッダ (1×10PIN)
- JP2:ピンヘッダ (2×3PIN)
- ID1:Chip Indactor (フェライトビーズ)
- ID2:Chip Indactor (フェライトビーズ)
- ZD1:ツェナーダイオード3.6V ※3.3VだとI2Cが動かないので注意
- ZD2:ツェナーダイオード3.6V ※3.3VだとI2Cが動かないので注意
- C1:0.1uF
- C2:22pF
- C3:22pF
- C4:22uF〜
- R1:68-100Ω
- R2:68-100Ω
- R3:4.7KΩ（回路図は1.5KΩとなっていますが4.7KΩの方が安定します）
- R4:470-1KΩ
- LED1:LED
- Q1:16Mhz

# example

- [blink_h:MIDI-INを受けてLEDチカするスケッチ(Hybrid MIDI Version)](../../arduino/libraries/HybridMidiAttiny/examples/blink_h)
- [button_h:スイッチを押すとMIDI送信(Hybrid MIDI Version)](../../arduino/libraries/HybridMidiAttiny/examples/button_h)
- [controller_h:ボリュームを回すとMIDIコントロール送信(Hybrid MIDI Version)](../../arduino/libraries/HybridMidiAttiny/examples/controller_h)
- [sounder_h:シンセモドキ1号(Hybrid MIDI Version)](../../arduino/libraries/HybridMidiAttiny/examples/sounder_h)

# Licenses

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />この 作品 は <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">クリエイティブ・コモンズ 表示 4.0 国際 ライセンスの下に提供されています。</a>






