## 数据说明

### 一、 首页数据 
  
   1. 修改 home.json 文件
   2. home.json 数据结构说明
      
      | 参数名 | 描述信息 | 备注｜
      |:---|:---|:---|
      | ** ElectricityData **         | 供售电量数据 |  |
      | ** ErecoveryData **           | 电费回收数据|  |
      | ** IndustryMonData  **        | 业扩监控数据 |  |
      | ** OutageTimeData **          | 客户平均停电时间数据 |  |
      | ** MediumVoltageFaultData **  | 中压线路故障率数据 |  |
      | ** DefectManageData **        | 缺陷隐患管理数据 |  |
      | ** currentWarningData **      | 95598当日预警数据 |  |
      | ** AutoMeteringMonitorData ** | 计量自动化监控数据 |  |
      | ** LineLossData **            | 同期线损数据 |  |
      | ** mapData **                 | 中间地图数据 |  |


      （1） ElectricityData 数据说明

      | 参数名 | 描述信息 | 备注｜
      |:---|:---|:---|
      | ** supply **           | 供电量数据 |  |
      | ** sellElectricity **  | 售电量数据|  |

      （2） ErecoveryData 数据说明

      | 参数名 | 描述信息 | 备注｜
      |:---|:---|:---|
      | ** recoveryRate **        | 回收率数据 |  |
      | ** oweAmount **           | 欠费金额|  |
      | ** currentYearData **     | 今年电费回收折线图 |  |
      | ** lastYearData **        | 去年电费回收折线图 |  |
      | ** beforeLastYearData **  | 前年电费回收折线图|  |

      （3） IndustryMonData 数据说明

      | 参数名 | 描述信息 | 备注｜
      |:---|:---|:---|
      | ** listData **      | 第一排数据 |  |
      | ** pieCharData1 **  | 第一个饼图数据 |  |
      | ** pieCharData2 **  | 第二个饼图数据 |  |
      | ** pieCharData3 **  | 第三个饼图数据 |  |

      （4） OutageTimeData 数据说明

      | 参数名 | 描述信息 | 备注｜
      |:---|:---|:---|
      | ** statisticsData **      | 柱状图（月、季、年值） |  completevalue:完成值（顺序：月、季、年）,cumulativevalue:累计值（图标是堆叠图，此项的值 = 累计值 - 完成值。顺序：月、季、年）|
      | ** targetLineChart **  | 折线图中的目标值 |  |
      | ** completeLineChart **  | 折线图中的完成值 |  |
      | ** rank **  | 排名 | 必须写5个 |
      
      （5） MediumVoltageFaultData 数据说明

      | 参数名 | 描述信息 | 备注｜
      |:---|:---|:---|
      | ** circleData **        | 圆形图数据 | 顺序：当年故障次数、当季故障次数、当月故障次数  |
      | ** completeData **      | 折线图中的完成值 |  |
      | ** completeLineData **  |折线图中的目标值 |  |
      | ** rank **              | 排名 | 必须写5个 |


      （6） DefectManageData 数据说明

      | 参数名 | 描述信息 | 备注｜
      |:---|:---|:---|
      | ** indicatorsData **  | 各项指标数据 | 顺序：紧急、重大、超期、预警、一般、其他   |
      | ** others **          | 最后一排数据 |  |

      （7） currentWarningData 数据说明

      | 参数名 | 描述信息 | 备注｜
      |:---|:---|:---|
      | ** yesterday **  | 昨日数据|  |
      | ** today **      | 今日数据|  |

      （8） AutoMeteringMonitorData 数据说明

      | 参数名 | 描述信息 | 备注｜
      |:---|:---|:---|
      | ** tabList **                   | 第一排数据|  |
      | ** pieData **                   | 环形图数据|  |
      | ** automaticData **             | 自动抄表数据|  |
      | ** terminalCoverageRateData **  | 终端覆盖率数据|  |

      （9） LineLossData 数据说明（直接看结构）

      （10） mapData 数据说明

      | 参数名 | 描述信息 | 备注｜
      |:---|:---|:---|
      | ** left **  | 左侧数据|  |
      | ** right ** | 右侧数据|  |

       left 左侧数据
      | 参数名 | 描述信息 | 备注｜
      |:---|:---|:---|
      | ** userData **          | 用户数 |  |
      | ** customerManager **   | 客户经理数 |  |
      | ** monitorService **    | 95598诉求 | orderQuantity：工单量，monthToMonthRatio：同比， yearToYearBasis：环比 |
      | ** pieCharData **       | 饼图数据 |  |
      | ** overtimeWorkOrder ** | 超时工单量 |  |



      right 右侧数据
      | 参数名 | 描述信息 | 备注｜
      |:---|:---|:---|
      | ** powerLine **               | 停电线路 | plan：计划，noInPlan：非计划  |
      | ** powerDistributionChange ** | 停电配变 | plan：计划，noInPlan：非计划  |
      | ** powerCuts **               | 停电计划 |  |
      | ** workPlan **                | 作业计划 | weekPlan：周计划，monthPlan：月计划 |
      | ** repairOrder **             | 稽查工单 | total：在途工单量，pieCharData：饼图数据 |

      

