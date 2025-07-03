# Shogunate-Policy-Beta (1.0)
# Shogunate-Pillar-of-Buka-Flavour (2.0)

互动计谋开发流程：

1、common\schemes\scheme_types中确定计谋类型

2、common\character_interactions中确定互动框架：通常一个为自体计谋，一个为委任计谋

3、events\scheme_events中确定计谋事件

4、localization\pob_schemes中本地化

政策开发流程：

1、common\scripted_effects\SP_00_init_flag_effects
这个文件定义了每个类型政策的flaglist，需要把新的政策作为flag加入list，flag当作便利的var使用

2、common\scripted_effects\SP_01_intro_policy_effects
这个文件定义了发布政策和撤销政策的效果，以及政策的花费，最后一个sp_set_policy_effects_to_character_effect是元effect，可以不用理会

3、common\scripted_triggers\SP_02_legacy_trait_triggers\sp_can_release_policy_trigger中确定能发布政策的条件

4、common\script_values\SP_03_values中确定需要消耗的政策点

