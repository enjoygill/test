1.git�����ϴ������ļ���.ssh�ļ���C:\Users\Administrator\.ssh
2.��һ���ڴ��ļ��м��㽨���Ĳֿ��У�����Ҽ�git bash ��Ȼ��Git init,
��������ssh -T git@github.com �����Ƿ�������github�ɹ�
����ǵ�һ�ξ���Ҫ����git����git������֪���㣻
 ��1�����ñ���ssh key
$ ssh-keygen -t rsa -C "1873247496@qq.com" github��ע�������
 ��2���ѱ������ɵ�key���Ƶ�github�ٷ���վssh key��
�ٴ���֤ssh -T git@github.com �����Ƿ�������github�ɹ�
3.ע������㽨���²ֿ�ʱ�򣬱��������û��������䣬��git֪������˭
$ git config --global user.name "enjoygill"
$ git config --global user.email "1873247496@qq.com"


--------------------------------�����ǵ�һ��������������ǵ�һ��ֱ�Ӵ�4��ʼ
4����������Ѿ����ã�ֱ��git remote add origin git@github.com:enjoygill���û�����/�ֿ�����test��.git
5.ÿ��׼���ϴ�ʱ����git pull�£�����ᱨ��ͬʱ,commit��ע��git status�鿴״̬
git add +�ύ���ݣ���ӵ���������
git commit -m "message" 
git push origin master   �������������������ύ��

6�������colne���صĻ�����Ҫ�½�һ���ļ��У�����gitbash������git init
�ڴ�������git clone git@github.com:enjoygill/��Ŀ����.git ��һ�㲻��ֱ��clone�ֿ��ĳ���ļ���  

7��Զ�̷�������¡һ��һģһ���İ汾�⵽����,���Ƶ��������汾�⣬����clone.
��clone�ǽ�һ���⸴�Ƶ���ı��أ���һ�����ش��޵��еĹ��̣�
 ��Զ�̷�������ȡ��һ��branch��֧�ĸ��µ����أ������±��ؿ⣬����pull.
��pull��ָͬ��һ�����㱾���а汾�Ŀ����ݸ��µĲ��ֵ���ı��ؿ⣩
 git pull�൱���Ǵ�Զ�̻�ȡ���°汾��merge���ϲ���������     
 git pull = git fetch + git merge��git fetch����ȫһЩ

8�޸ģ���clone���غ�Ҫ�޸ĺ������Ҫ�ύ�������ȱ��浽�ݴ����������ύ��ȥ��
Ҫ�ȼ��뵽 staging area �ĸĶ��Żᱻ git commit �ύ��ͬһ���ļ�Ҳ���� add ��Ρ�
����add���ԣ�
git commit -m 'msg' <file>
����
git commit -m 'msg' -a