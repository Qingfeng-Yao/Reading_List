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
- simhash: �������ӳ�������֮��ĽǶ�, 
![simhash�����ѧ����](images/simhash.jpeg)


## �ο�����
- Hashing for Similarity Search: A Survey
- Detecting Near-Duplicates for Web Crawling