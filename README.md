# 数据库(data base)

- mysql可视化工具 navicat

dbpath:数据文件存放路径，每个数据库会在其中创建一个子目录，用于防止同一个实例多次运行的mongod.lock也保存在此目录中。

logpath:错误日志文件。

logappend：错误日志采用追加没模式（默认是覆写模式）。

bind_ip:对外服务的绑定Ip，一般设置为空，及绑定在本机所用可用Ip上，如有需要可以单独指定。

port：对外服务端口，web管理端口在这个port的基础上+1000.

fork：以后台Daemon形式运行服务。

journal：开启日志功能，通过保存操作日志来降低单机故障的恢复时间，在1.8版本后正式加入，取代在1.7.5版本中的dur参数。

syncdelay：系统同步刷新磁盘的时间，单位为秒，默认是60秒。

directoryperdb：每个db存放在单独的目录中，建议设置该参数。

maxConns：最大连接数。

repairpath：执行repair时的临时目录。如果没有开启journal，异常down机后重启，必须执行repair操
