### �������� ����� ��������� ������

������� floor: ������� ������, ��� ���� ��������� �������� ���� "������", "������" � �.�., �.�. �� ���� ������ ��������. ������� floor �������������� � �������������� ������� � ����������� ����������: first/basement/higher_floor/multy_level � unknown ��� ����������� ��������.

�������: reform_house_population_1000', 'reform_house_population_500','reform_mean_floor_count_1000', 'reform_mean_floor_count_500','reform_mean_year_building_1000', 'reform_mean_year_building_500', � ��� �������� ��������� �������� �� ������/�������.

�������������� ������: �������� ������ ����������������. (������: https://www.klerk.ru/tools/refinancing/)

### �������� �������� �������� � ��������� ����������
������� ������ ������ �� �������, ��� price_type = 1.
������ ������� ���������� � ������������ �������� (catboostregressor) c depth = 12, iterations = 900
�������� score = �� ����� ��������� �� ����. ���� ���� � 21-45
� ������ ��������������� ������������ 0,9:
test_predict_corrected = test_predict*0.9