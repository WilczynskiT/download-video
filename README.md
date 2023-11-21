# PizzaBaker

Copyright © 2023 Tomasz Wilczyński. All Rights Reserved.

License: AGPL-3.0

https://wilcz.com


Welcome!

It is bash script to download video chunks and merge it into single .ts file.
It could be use to capture videos from websites where it is not possible from UI.

====================== PizzaBaker.sh ==============================
PizzaBaker.sh [-t] [Video URL with {no}]

Instruction:

1. open webpage with video, set quality, skip ads and pause video

2. open inspector

3. go to network tab

4. play video

5. find element like cdn, with extesion .ts or similar, example: https://d2vn0zi4e5kfuy.cloudfront.net/prod/binary/2023/11/20/21/art_7447072/1595772789217-jugr68/2011N376XR_dssa_da**11**.ts

6. next elements should have higher numbers (nex chunks) like: https://d2vn0zi4e5kfuy.cloudfront.net/prod/binary/2023/11/20/21/art_7447072/1595772789217-jugr68/2011N376XR_dssa_da**12**.ts

7. replace number with "{no}", example: https://d2vn0zi4e5kfuy.cloudfront.net/prod/binary/2023/11/20/21/art_7447072/1595772789217-jugr68/2011N376XR_dssa_da**{no}**.ts

8. run: PizzaBaker.sh "https://d2vn0zi4e5kfuy.cloudfront.net/prod/binary/2023/11/20/21/art_7447072/1595772789217-jugr68/2011N376XR_dssa_da{no}.ts"

9. wait until terminal finish work 

10. done! you can convert this video from ts to mp4 using external software or play it using VLC media player

*If you want to check temporary files use -t, they will not be deleted.*

