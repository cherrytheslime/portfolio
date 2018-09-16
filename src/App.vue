<template>
  <div id='app'>

    <div class='view'>

      <portfolio></portfolio>

    </div>

  </div>
</template>

<script>
import Portfolio from '@/components/portfolio'

export default {
  name: 'app',
  components: { Portfolio },
  data () {
    return {
    }
  },
  mounted() {
    const strings = ['do you like our owl?', 'gimmie pizza', 'pc load letter what the fuck does that mean?'],
      randomIndex = Math.floor(Math.random() * strings.length),
      skeleStrings = strings[randomIndex],
      skele = '                       :::!~!!!!!:.\n' + '                    .xUHWH!! !!?M88WHX:.\n' + '                 .X*#M@$!!  !X!M$$$$$$WWx:.\n' + '                :!!!!!!?H! :!$!$$$$$$$$$$8X:\n' + '               !!~  ~:~!! :~!$!#$$$$$$$$$$8X:\n' + '              :!~::!H!<   ~.U$X!?R$$$$$$$$MM!\n' + '              ~!~!!!!~~ .:XW$$$U!!?$$$$$$RMM!\n' + '              ~!~!!!!~~ .:XW$$$U!!?$$$$$$RMM!\n' + '                !:~~~ .:!M"T#$$$$WX??#MRRMMM!\n' + '                ~?WuxiW*`   `"#$$$$8!!!!??!!!\n' + '              :X- M$$$$       `"T#$T~!8$WUXU~\n' + '             :%`  ~#$$$m:        ~!~ ?$$$$$$\n' + '           :!`.-   ~T$$$$8xx.  .xWW- ~""##*"\n' + ' .....   -~~:<` !    ~?T#$$@@W@*?$$      /`\n' + ' W$@@M!!! .!~~ !!     .:XUW$W!~ `"~:    :\n' + ' #"~~`.:x%`!!  !H:   !WM$$$$Ti.: .!WUn+!`\n' + ' :::~:!!`:X~ .: ?H.!u "$$$B$$$!W:U!T$$M~\n' + ' .~~   :X@!.-~   ?@WTWo("*$$$W$TH$! `\n' + ' Wi.~!X$?!-~    : ?$$$B$Wu("**$RM!\n' + '$R@i.~~ !     :   ~$$$$$B$$en:``\n' + '?MXT@Wx.~    :     ~"##*$$$$M~    ' + skeleStrings +' \n';
    console.log(skele)
  }
}
</script>
