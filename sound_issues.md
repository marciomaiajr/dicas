# Problema com o som ALSA e Pulseaudio

## Problema de sound crackling no desktop 

Solução para o problema de **sound crackling** na saída de áudio line-out do desktop, codec Realtek ALC892

adicionar a linha abaixo:

```
options snd-hda-intel model=dell-headset-multi
```

no arquivo:

```
/etc/modprobe.d/alsa-base.conf
```
e reiniciar o computador.

fonte: 
[https://askubuntu.com/questions/1258583/install-realtek-audio-drivers-in-ubuntu-20-04-intel-nuc-nuc10i7fnh](https://askubuntu.com/questions/1258583/install-realtek-audio-drivers-in-ubuntu-20-04-intel-nuc-nuc10i7fnh)
[https://community.intel.com/t5/Intel-NUCs/NUC10i5-headphones-jack-audio-not-working-with-Ubuntu-20-04/td-p/643946](https://community.intel.com/t5/Intel-NUCs/NUC10i5-headphones-jack-audio-not-working-with-Ubuntu-20-04/td-p/643946)
