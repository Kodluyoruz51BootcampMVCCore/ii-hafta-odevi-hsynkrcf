# GİTHUB

### Github Nedir?

GitHub, git yazılımı ile entegre olmuş bir depolama alanıdır. Git ile GitHub birbirine karıştırmayın lütfen. Git versiyon kontrol sistemidir. GitHub sayesinde dünyanın çeşitli ülkelerinden, bu ülkelerin bazı yerlerinden, projenize farklı bir kaç kişi ekleyerek takım çalışması yapabilirsiniz. Ayrıca, GitHub ile dünya üzerinde projenizin herkes tarafından görülmesini, değerlendirilmesi sağlayabilirsiniz. GitHub üzerinde paylaşılan kodlar ile kendinizi geliştirebilirsiniz.

### GitLab Nedir?

GitLab, GitHub’ın kullanıcılara sağladığı işlevlerin tamamını sunan bir Git servisidir.Açık kaynak(open source) projelerinizi bu servis üzerinde ücretsiz bir şekilde oluşturabilir ve yönetebilirsiniz. GitLab daha çok firmalarda tercih ediliyor çünkü : Ücretsiz sürümünde kendi sunucularınıza kurarak sadece kurum içi kullanıcıların erişebileceği GitLab servisi hizmeti bulunmaktadır.

### Bitbucket Nedir?

Bitbucket, Git veya Mercurial sürüm kontrol sistemi kullanan projeler için bir ağ depolama servisi olup Django kullanılarak Python programlama dili ile yazılmıştır. Bitbucket, hem ticari planlarla hem de ücretsiz hesaplarla kullanılabilir.

### GitKraken Nedir?

Axosoft’un ürünü olan git projelerin yönetilmesinin kolaylaştıran ve branch’ların görsel olarak görünmesini sağlayan masaüstü uygulamasıdır. [www.gitkraken.com](http://www.gitkraken.com/) adresinden yazılıma ulaşılabilir. Yazılımı kişisel projelerde ve open-source projelerde kullanmak ücretsizdir.

# GitFlow vs GitHub Flow

GIT'de bir yazılımı yönetmenin başlıca yolları şunlardır: Git Akışı ve Github Akışı.
Bu 2 yöntem, projenizi yönetmenize ve ekipteki iş akışınızı optimize etmenize gerçekten yardımcı olabilir.
Aralarındaki farkları görelim.

## GitFlow
![GitFlow Photo](https://i2.wp.com/lanziani.com/slides/gitflow/images/gitflow_1.png?zoom=2)

Git flow works with different branches to manage easily each phase of the software development, it’s suggested to be used when your software has the concept of “release” because, as you can see in the scheme above, it’s not the best decision when you work in Continuous Delivery or Continuos Deployment environment where this concept is missing.
Another good point of this flow is that fits perfectly when you work in team and one or more developers have to collaborate to the same feature.
But let’s take a look closer to this model.

The main branches in this flow are:

- master
- develop
- features
- hotfix
- release

## GitHub Flow
![GitHub Flow Photo](https://lucamezzalira.files.wordpress.com/2014/03/screen-shot-2014-03-08-at-23-07-361.png?w=768&h=272)

So now, do you think that Github is working with Git Flow? Of course no! (Honestly I was really surprised when I read that!)
In fact they are working with a continuos deployment environment where there isn’t the concept of “release” because every time they finish to prepare a new feature they push live immediately (after the whole automation chain created in the environment).
The main concepts behind the Github flow are:

- Anything in the master branch is deployable
- To work on something new, create a descriptively named branch off of master (ie:new-oauth2-scopes)
- Commit to that branch locally and regularly push your work to the same named branch on the server
- When you need feedback or help, or you think the branch is ready for merging, open a pull request
- After someone else has reviewed and signed off on the feature, you can merge it into master
- Once it is merged and pushed to ‘master’, you can and should deploy immediately


KAYNAK : https://lucamezzalira.com/2014/03/10/git-flow-vs-github-flow/
KAYNAK : https://www.tolgacibikci.com/git-nedir-nasil-kurulur/
