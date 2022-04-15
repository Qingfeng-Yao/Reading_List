## ����˼��
### �ı�ȥ������
- Near-duplicate Detection / Similarity Search
- ��Ҫ���ı�ȥ�ط���������:
    - ���������Եķ���: ���ݻ�ṹ������, ���ݰ����ַ���ƥ��(Shingling)��������������(TF/TFIDF)
    - ����ժҪ�����ķ���: �ı�������ȡ+ժҪ����(��ϣ)
        - �ֲ����й�ϣ(Locality Sensitive Hashing)
        - ��ϣѧϰ(Learning to Hash)
        - ���������Ƿ�������ݷֲ�ѧϰ��ϣ����
- LSH: ����һ���ϣ�����Ķ���, ��Щ�������Ը��ߵĸ��ʽ����Ƶ�������ӳ�����ͬ�Ĺ�ϣ��(�������Ƶ�������)
    - ������һ���ϣ����һ����Բ�ͬ�ľ���������Զ���, ������Ի��ڽǶ�(angle-based)�ľ��붨���sign-random-projection(or simhash)
- simhash: �������ӳ�������֮��ĽǶ�
    - ����ӳ��: �����ڴ��ģ����, �ܿ�������
![simhash�����ѧ����](images/simhash.jpeg)
- ʵ��ָ��
    - mean average precision(MAP): mean���������query���Ե�, ��Ҫ��ÿ��query����average precision, �����ÿ��query�õ��������б�ͳ���������item��precision�ľ�ֵ; ÿ�����item��precision������Ҫ���������item�����Ҵ�1-len(items)��֣�������item��Ӧ������λ��(��Ҫ+1)
    - P_R����: P��R���ǳ���Ϊcode_length���б�, �����α���ÿ��query����һ��PR�б�Ȼ�����ֵ; ÿ��PR�б���ͨ����ÿ��codeλ��Ϊ��ֵ������õĺ��������������
![MAP example](images/map.jpg)


## �ο�����
- Hashing for Similarity Search: A Survey
- Detecting Near-Duplicates for Web Crawling