## User（用户类）

- user_id：用户id（key）
- user_name：用户姓名
- sex：用户性别
- nickname：用户昵称
- city_id：城市id
- chosen_role_id：用户选择角色的id（默认为初始角色形象）enum枚举类型
- BWT_TH_GAME_ID：用户解锁关卡的id
- BWT_TH_STATION_ID：用户到达的站点id

## Score（积分类）

- user_id：用户id（foreign key）

- user_score：用户积分
- user_co2_score：用户碳排放量积分

## Medal（勋章类）

- user_id：用户id（foreign key）
- medal_type：勋章类别
- message_finished：是否显示勋章（true/false）

## Message（信息类）

- user_id：用户id（foreign key）
- message_id：信息id
- message_type：信息所属类别（13号线，10号线等等）
- message_content：信息描述
- message_collected_id：用户已收集信息id
- message_not_collected_id：用户未收集信息id
- message_finished：是否全部收集（true/false）

## Products（商品类）

- product_id：商品id（key）
- product_price：商品价格
- product_description：商品描述