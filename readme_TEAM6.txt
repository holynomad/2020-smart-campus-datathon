#================= 2020 KU ����Ʈ ķ�۽� �������� 6�� [SKUM - Safe Korea Univ. Map, "����"] readme_TEAM6.txt ====================
#================= �ڡ� ���� �ڡ� readme ��� �� public ������ ����� �κ��� ���ܵ� 

# !���� [00.readme_TEAM6]�� TEAM6_OUTPUT_DIR_STRUCTURE.png ������ ���� ��ü���� ���⹰ ��Ʈ��ó�� ���캾�ϴ�.

# ������ �� ���⹰ ������ �Ʒ��� �����ϴ�.

	[01.�ǿ� ������ �����ͼ� ũ�Ѹ�(API)]
	
		[A.���û ���׿�����ȸ(API)]
		
			���û18_���׿��� ��ȸ����_����APIȰ�밡�̵�.docx - ���û���� ������ ����API ���̵��
			airAPI.py - ���û ������ API ũ�Ѹ� �ҽ�(Python)
			air_output_sample_10000row.csv - ũ�Ѹ� �������(7/30 ���� 3����ġ)
		
		[B.�ѱ�ȯ����� ����������(API)]
		
			airkorea_openapi_guide-v1_7_2.docx - �ѱ�ȯ����ܿ��� �����ϴ� �ǿܴ����� ������ ����API ���̵��
			weatherAPI.py - �ǿܴ����� ������ API ũ�Ѹ� �ҽ�(Python)	
	
	[02.��������ó�� �� ���յ����ͼ� ����]
	
		[A.IoT �����ͼ� ��ȯ(txt2csv)]
		
			txt2csv.py - �������� ����ο��� �������� SK�̷��� IoT���� �������� Text-to-CSV ��ȯ �ҽ�(Python)
			�� �� Input (TXT) & Output ����(CSV)
		
		[B.SK�̷��� ���� �뺰������ ���� �� ���Capa�󺧸�]
		
			skf_area_tot.csv - SK�̷��� ���� �뺰 ���鿡�� �뺰-Size���� ����/����� �����ͼ�
			label_capaNpcnt_iot_n_airinfo_200812.R - �� �����ͼ°� [02-A]�ܰ迡�� ��ȯ�� IoT �����ͼ�(CSV)�� roomid�� �����ϰ� ���� ����ο�(personCnt) �󺧸� �ҽ�(R)
			area_pcnt_rnorm_merged_20200618_v1.1.csv �� 2�� - �ش� �������
			
		[C.�ǳ�(IoT)+�ǿ�(API) ���յ����ͼ� ����]
		
			merge_iot_n_airinfo_200805.R - [02-B]�ܰ迡�� ������ IoT �����ͼ°� [01]�ܰ迡�� ������ �ǿܴ����� �����ͼ�(API) ���� �ҽ�(R)
			iot_air_merged_20200611.csv �� 3�� - �� �ҽ� �������
			merge_all_linked_200820.R - �� ���ں� �����ͼ�(CSV)�� �ϳ��� ���Ϸ� ������ �ҽ�(R)
			iot_allmerged_0618_0702.csv - �� �ҽ� �������
			
		[D.Ž���� ������ �м�]
		
			EDA.R - �ǳ�+�ǿ� ���յ����ͼ� ��� Ž���������ͺм� �ǽ��� �ҽ�(R)
	
	[03.���� DR�ó����� �󺧸� �� �ð�ȭ]
	
		[A.SK�̷��� �ǹ� �����̹���]
		
			�������� ����ο��� �������� SK�̷��� ����(B1F~5F) �뺰 ��������(PDF)
			SKUM_COVID���赵_UI����.png - �� �����̹��� �м��� �������� SKUM UI ���� �̹���
			 
		[B.���� DR �ó����� ���̽� �󺧸�]
		
			�󺧸� ����_20200820_heatmap���� 5�ܰ�.xlsx - ���� DR �ó����� ���̽��� �󺧸� ���� ��ü�м�ǥ
			label_all_Y_merged_200826.R - �� ���ؿ� ���� ������ ���� DR �ó������� �󺧸� �ҽ�(R)
			labelled_all_merged_0618_0702_v1.0.csv - �� �ҽ��� �������� 6/18~7/2 �ǳ�(IoT)+�ǿ�(API) ���� �����ͼ� �󺧸� �������
			
		[C.�ð�ȭ(Heatmap + 2D Gaussian)]
		
			heatmap_01.py - Ư�� feature�� (��: dust, temp, humid, covid_case��) �뺰(roomid) �ð迭 �ð�ȭ(heatmap, Python)
			Figure_1_COVID Risk TimeSeries Map_0625~0702_marked.png - heatmap_01.py ���� COVID �������赵(covid_case) �뺰-�ð迭 heatmap ������� �̹���
			heatmap_02.py - SK�̷��� 2F �����̹����� ������ �� Ư�� �뺰(roomid) Ư�� ���� DR �ó����� feature (��: covid_case, di_case, complx_case ��)�� 2D Gaussian �ð�ȭ ���� �ҽ�(Python)
			2F.png - SK�̷��� 2F ���� �̹���
			Figure_2_SKF_2F_COVID_RISK_MAP(sample).png - SK�̷��� 2F Ư�� ���͵���� COVID �������赵 �ð�ȭ ���� �̹���
			Figure_3_SKF_2F_COMPLX_RISK_MAP(sample).png - SK�̷��� 2F Ư�� ���͵���� COVID ������ �ð�ȭ ���� �̹���
			Figure_4_SKF_2F_DI_MAP(sample).png - SK�̷��� 2F Ư�� ���͵���� ��������(���赵) �ð�ȭ ���� �̹���
			heatmap_03.py - �� heatmap_02.py�� �ڵ� �ִϸ��̼����� �ð迭 �ð�ȭ �����ϱ� ���� �ҽ�(�̿ϼ�, Python)
			Figure_5_COVID_Virtual labelled Dataset.png - heatmap_02.py �� heatmap_03.py���� 2D Gaussian �ð�ȭ�� ���� ����� ���õ����ͼ� ����ĸ�� �̹���
			
	[04.SKUM�� ������Ÿ����]
	
		SKUM UI Flow_v2_20200823.pptx - SKUM�� ��ȹ�� �ۼ��� UX ���̵���ο� ���� �������� �� UI flow
		SKUM Prototype_v1.0.mp4 - �� UI flow�� �������� ����� �� SKUM �� ���𿵻�(��1��30��, Adobe Xd)
		SKUM LivingLab Prototype v1.0.mp4 - ������Ʈ�� �糭����(DR) ������ ������ ���� SKUM ������ �� ���𿵻�(��1��30��, Adobe Xd)
	
	[99.�м��𵨸� ���� ������]
	
		������ �м� �� ���� DR �ó����� (COVID ��������, ȭ������, ���������� ��) �󺧸� ���� ������ �ڷ��(PDF)
	
