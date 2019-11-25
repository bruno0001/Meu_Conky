#Meu Conky
#Conky, a system monitor, based on torsmo
#alignment top_right # middle_right
background no
use_xft yes
font Dejavu Sans:size=9
xftalpha 0
update_interval 2.0
total_run_times 0
own_window yes
own_window_transparent no
own_window_type desktop
own_window_argb_visual yes
own_window_argb_value 120
own_window_hints undecorated,below,sticky,skip_taskbar,skip_pager
double_buffer yes
#minimum_size 200 200
#maximum_width 300 #200
draw_shades no
draw_outline yes
draw_borders no
draw_graph_borders yes #no
default_color 999999
default_shade_color black
default_outline_color black
alignment top_right
gap_x 8 #8
gap_y 124
no_buffers yes
cpu_avg_samples 2
text_buffer_size 1024
override_utf8_locale no
uppercase no
double_buffer yes

TEXT
S I S T E M A
$hr
Sistema: $sysname $kernel
${color grey}Tempo escedido:$color $uptime
Hora: ${time %H:%M:%S} Data: ${time %e/%b/13}
C P U$alignr ${cpu cpu0}%
$hr
Procesador: ${alignr}${freq_g}GHz / 2.28GHz
${color green}${cpubar 4 cpu0}${color grey}
${color green}${cpubar 4 cpu1}${color grey}
${color green}${cpubar 4 cpu2}${color grey}
${color green}${cpubar 4 cpu3}${color grey}
T O P C P U
$hr
Proceso$alignr CPU% MEM%
${top name 1}$alignr${top cpu 1} ${top mem 1}
${top name 2}$alignr${top cpu 2} ${top mem 2}
${top name 3}$alignr${top cpu 3} ${top mem 3}
R A M$alignr $memperc%
$hr
Memoria: ${alignr}${mem} / ${memmax}
${color green}${membar 4}${color grey}
T O P R A M
$hr
Proceso $alignr CPU% MEM%
${top_mem name 1}$alignr${top_mem cpu 1} ${top_mem mem 1}
${top_mem name 2}$alignr${top_mem cpu 2} ${top_mem mem 2}
${top_mem name 3}$alignr${top_mem cpu 3} ${top_mem mem 3}
A R M A Z E N A M E N T O
$hr
Raiz: ${alignr}$color${fs_used /} / ${fs_size /}
${color green}${fs_bar 4 /}${color grey}
Home: ${alignr}$color${fs_used /home} / ${fs_size /home}
${color green}${fs_bar 4 /home}${color grey}
4760CE7366471CEB: ${alignr}$color${fs_used /run/media/celsopassos/4760CE7366471CEB} / ${fs_size /run/media/celsopassos/4760CE7366471CEB}
${color green}${fs_bar 4 /run/media/celsopassos/4760CE7366471CEB}${color grey}
R E D E S${alignr}${downspeed wlp1s0}
$hr
Entrada/Saida ${alignr}${totaldown wlp1s0} / ${totalup wlp1s0}
