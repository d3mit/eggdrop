eggdrop
=======

Configuration.conf

# ----------------------------- Begin of Bot Setting's ----------------------------
set my-ip ""
set nick "Waria^Kuntet"
set owner "Fack"
set basechan "#scan"
set username "sempak"
# ------------------------------ End of Bot Setting's -----------------------------
###################################################################################
# ANDA SESUAIKAN 5 SETINGAN DI ATAS, KEMUDIAN JALANKAN EGGDROP ANDA DENGAN        #
# PERINTAH: ./eggdrop -m config.conf                                           #
#                                                                                 #
# SETELAH BOT ANDA ONLINE DI IRC, KETIKKAN PERINTAH DI BAWAH INI:                 #
# on IRC:  /msg BoTNICK pass <YourPassword>                                       #
#          /msg BoTNICK auth <YourPassword>                                       #
#          /msg BoTNICK botnick <botnick> <nickpass>                              #
#          /msg BoTNICK botaltnick <botnick> <nickpass>                           #
#                                                                                 #
# 4 PERINTAH DI ATAS ADALAH UNTUK PERTAMA KALI ANDA LOAD BOT, LOAD KEDUA DAN      #
# SETERUSNYA TIDAK PERLU DI SET LAGI, UNTUK MENGETAHUI SEMUA PERINTAH BOT KETIK   #
# PERINTAH: /msg BoTNICK help                                                     #
#                                                                                 #
###################################################################################

#########################
##### GENERAL STUFF #####
#########################
#set my-hostname "localhost"
set altnick "Irba"
set nickpass "hahahehe"
set altpass "hahahehe"
set cfgfile "${nick}.cfg"
listen 4000 all
set userfile "${nick}.usr"
set chanfile "${nick}.chn"
set admin "fack"
set kick-bogus-invites 1
set default-flags "hp"
set network "154.35.175.101"
set timezone "EST"
set max-logs 5
set max-logsize 0
set quick-logs 0
set log-time 1
set keep-all-logs 0
set switch-logfiles-at 300
set console "mkcobxs"
set sort-users 0
set notify-newusers "$owner"
set help-path "help/"
set text-path "text/"
set temp-path "help/"
set motd "text/motd"
set whois-fields "Powered FACK"
set realname "Powered FACK"
set protect-telnet 0
set dcc-sanitycheck 0
set ident-timeout 30
set mod-path "modules/"
loadmodule transfer
set require-p 0
set open-telnets 0
set stealth-telnets 1
set connect-timeout 15
set dcc-flood-thr 3
set telnet-flood 5:60
set resolve-timeout 15
set ignore-time 15
set debug-output 0
set hourly-updates 00
set remote-boots 2
set share-unlinks 1
set die-on-sighup 0
set die-on-sigterm 0
unbind dcc n tcl *dcc:tcl
unbind dcc n set *dcc:set
set must-be-owner 0
unbind dcc n simul *dcc:simul
set max-dcc 50
set dcc-portrange 1024:65535
set enable-simul 1
set allow-dk-cmds 1
loadmodule channels
set ban-time 30
set exempt-time 0
set invite-time 0
set share-greet 0
set use-info 1
set global-flood-chan 5:10
set global-flood-deop 3:10
set global-flood-kick 3:10
set global-flood-join 3:10
set global-flood-ctcp 2:10
loadmodule server
set net-type 3
set init-server { putserv "MODE $botnick +iw-s" }
set revenge-mode 1
set keep-nick 1
set use-ison 1
set strict-host 0
set quiet-reject 1
set lowercase-ctcp 0
set answer-ctcp 3
set flood-msg 5:60
set flood-ctcp 3:60
set never-give-up 1
set strict-servernames 0
set default-port 6667
set server-cycle-wait 40
set server-timeout 30
set servlimit 0
set check-stoned 1
set use-console-r 0
set serverror-quit 0
set max-queue-msg 300
set double-mode 0
set double-server 0
set double-help 0
set trigger-on-ignore 0
set use-silence 0
set check-mode-r 0
loadmodule ctcp
set ctcp-mode 0
loadmodule irc
set bounce-bans 1
set bounce-modes 0
set max-bans 20
set max-modes 30
set allow-desync 0
set kick-bogus 0
set ban-bogus 0
set kick-fun 0
set ban-fun 0
set learn-users 0
set wait-split 300
set wait-info 180
set mode-buf-length 200
unbind msg - hello *msg:hello
unbind msg - ident *msg:ident
set no-chanrec-info 0
set bounce-exempts 0
set bounce-invites 0
set max-exempts 0
set max-invites 0
set kick-method 1
set modes-per-line 3
set use-354 0
set max-dloads 3
set dcc-block 0
set copy-to-tmp 1
set xfer-timeout 30
loadmodule share
set allow-resync 0
set resync-time 900
set private-owner 0
set private-global 0
set private-globals "mnot"
set private-user 0
loadmodule filesys
set files-path ""
set incoming-path ""
set upload-to-pwd 0
set filedb-path ""
set max-file-users 20
set max-filesize 1024
loadmodule notes
set notefile "${nick}.nts"
set max-notes 50
set note-life 1
set allow-fwd 0
set notify-users 0
set notify-onjoin 0
loadmodule console
set console-autosave 1
set force-channel 0
set info-party 0
checkmodule blowfish
loadmodule assoc
loadmodule wire
##### TAMBAHKAN TCL KAMU DISINI #####################
source scripts/alltools.tcl
source scripts/ary.tcl
source scripts/userinfo.tcl
source scripts/ping.tcl
source scripts/shio.tcl
source scripts/horoskop.tcl
source scripts/ipcheck.tcl
source scripts/koclokz.tcl
source scripts/info.tcl
source scripts/jodoh.tcl
source scripts/portchk.tcl
source scripts/dns.tcl
source scripts/dwhois.tcl
source scripts/google.tcl
