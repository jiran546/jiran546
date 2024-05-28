with open('Export_Output_21.json') as f:
    data = json.load(f)
m = folium.Map([30.9756, 112.2707], zoom_start=10)  # 设置地图的初始中心位置和缩放级别
m = folium.Map([30.9756, 112.2707], zoom_start=10)  # 创建地图对象并设置初始中心位置和缩放级别
folium.GeoJson(data).add_to(m)  # 将 .json 数据添加到地图上
m.save('map.html')  # 保存地图为 HTML 文件
m  # 显示地图
m = folium.Map(location=[30.9756, 112.2707], zoom_start=10, tiles='Stamen Toner')  # 使用 Stamen Terrain 风格的地图
folium.GeoJson(data).add_to(m)  # 将 .json 数据添加到地图上
m.save('map.html')  # 保存地图为 HTML 文件
m  # 显示地图
