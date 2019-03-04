
1. (ok )  `wav` to `midi` with [waon](https://github.com/kichiki/WaoN)
2. (no )  change instrument with `rosegarden` (sucks though, figure out how to do it manually)
3. (no )  create 2 `midi` with `helicopter` and `woodblock`
4. (ok?)  convert to `wav`
5. (ok?)  kill clippy stereo channel (right?)
6. (ok?)  mix tracks (woodblock at 80% vol) `audacity` (sucks though, combine tracks in midi?)
7. (ok?)  normalize `audacity`, sucks though

should be able to do everything with `waon`, `sox`, 

### mix waves (maybe do it at midi though) (figure out volume)

`sox -M heli.wav myrecording.wav output_test.aiff`

### get left

`sox infile.wav outfile.l.wav remix 1`

### normalize 

`sox −−norm=−3 infile outfile`

### get bytes

`xxd -i somefile.wav > somefile_wav.h`
