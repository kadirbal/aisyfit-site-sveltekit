<script lang="ts">
	import { getLocale } from '$lib/paraglide/runtime';
</script>

<div class="mx-auto prose max-w-4xl prose-invert prose-green">
	{#if getLocale() === 'tr'}
		<h1>AisyFit için Gizlilik Politikası</h1>
		<p><strong>Son Güncelleme:</strong> 5 Ocak 2026</p>

		<h2>1. Giriş</h2>
		<p>
			<strong>AisyFit</strong> ("biz", "bizim" veya "bize") olarak gizliliğinizi korumaya ve mobil uygulamamız
			ile hizmetlerimizde (topuca "Hizmet") olumlu bir deneyim yaşamanızı sağlamaya kararlıyız.
		</p>
		<p>
			Bu Gizlilik Politikası, yapay zeka destekli fitness koçluğu uygulamamızı kullandığınızda
			bilgilerinizi nasıl topladığımızı, kullandığımızı, açıkladığımızı ve koruduğumuzu açıklar.
			Lütfen bu gizlilik politikasını dikkatlice okuyun. Eğer bu gizlilik politikasındaki şartları
			kabul etmiyorsanız, lütfen uygulamaya erişmeyin.
		</p>

		<h2>2. Topladığımız Bilgiler</h2>
		<p>
			Sizi tanımlayan, sizinle ilişkilendirilebilen veya doğrudan ya da dolaylı olarak sizinle
			bağlantı kurulabilecek bilgileri ("Kişisel Bilgiler") topluyoruz.
		</p>

		<h3>A. Bize Sağladığınız Bilgiler</h3>
		<ul>
			<li><strong>Hesap Kaydı:</strong> İsim, e-posta adresi, şifre ve profil fotoğrafı.</li>
			<li>
				<strong>Sağlık ve Fitness Verileri:</strong> Cinsiyet, yaş, kilo, boy, aktivite seviyesi, fitness
				hedefleri, beslenme tercihleri, alerjiler, sakatlıklar ve antrenman geçmişi.
			</li>
			<li>
				<strong>Kullanıcı İçeriği:</strong> Geri bildirimler, günlükler, check-in'ler ve yüklediğiniz
				fotoğraflar (örn. gelişim fotoğrafları).
			</li>
		</ul>

		<h3>B. Otomatik Olarak Toplanan Bilgiler</h3>
		<ul>
			<li>
				<strong>Cihaz Bilgileri:</strong> Cihaz türü, işletim sistemi, benzersiz cihaz kimlikleri (örn.
				IDFA, Android ID) ve IP adresi.
			</li>
			<li>
				<strong>Kullanım Verileri:</strong> Uygulamamızı ziyaret detaylarınız, trafik verileri, günlükler
				(loglar) ve eriştiğiniz kaynaklar.
			</li>
			<li>
				<strong>Metrikler:</strong> İşlevsellik etkinleştirildiyse ve izinler verildiyse; günlük adım
				sayıları, su tüketimi ve diğer takip edilen metrikler.
			</li>
		</ul>

		<h3>C. Yapay Zeka (AI) İşleme</h3>
		<ul>
			<li>
				Kişiselleştirilmiş antrenman ve diyet planları oluşturmak için Yapay Zeka (AI) kullanıyoruz.
				Sağladığınız veriler (hedefler, sakatlıklar, tercihler), bu planları oluşturmak için AI
				algoritmalarımız tarafından işlenir.
			</li>
		</ul>

		<h2>3. Bilgilerinizi Nasıl Kullanıyoruz</h2>
		<p>Topladığımız bilgileri aşağıdaki amaçlarla kullanıyoruz:</p>
		<ul>
			<li>
				<strong>Hizmeti Sağlamak ve Yönetmek:</strong> Kişiselleştirilmiş hesap profilleri oluşturmak,
				AI destekli antrenman ve diyet planları üretmek ve gelişiminizi takip etmek.
			</li>
			<li>
				<strong>Hizmeti Geliştirmek:</strong> Kullanım modellerini analiz etmek, AI modellerimizi eğitmek
				(anonimleştirilmiş veriler üzerinde) ve hataları gidermek.
			</li>
			<li>
				<strong>İletişim:</strong> Size güncellemeler, güvenlik uyarıları ve destek mesajları göndermek.
			</li>
			<li>
				<strong>Uyumluluk:</strong> Yasal yükümlülüklere uymak ve Kullanım Koşullarımızı uygulamak.
			</li>
		</ul>

		<h2>4. Sağlık Verileri İçin Özel Hükümler</h2>
		<p><strong>AisyFit</strong>, sağlık ve fitness verilerinize yüksek hassasiyetle yaklaşır.</p>
		<ul>
			<li>Kişisel sağlık verilerinizi üçüncü taraflara <strong>satmayız</strong>.</li>
			<li>
				Sağlık verilerinizi yalnızca uygulamanın fitness ve beslenme koçluğu özelliklerini sağlamak
				için kullanırız.
			</li>
			<li>
				Apple HealthKit veya Google Fit ile entegrasyon sağlarsanız, bu verileri yalnızca uygulama
				içindeki gelişiminizi güncellemek için kullanırız ve reklam amacıyla kullanmayız.
			</li>
		</ul>

		<h2>5. Bilgilerinizin Paylaşımı</h2>
		<p>Bilgilerinizi şunlarla paylaşabiliriz:</p>
		<ul>
			<li>
				<strong>Hizmet Sağlayıcılar:</strong> Bizim adımıza hizmet veren üçüncü taraf tedarikçiler:
				<ul>
					<li>
						<strong>Supabase:</strong> Güvenli veritabanı barındırma ve kimlik doğrulama için.
					</li>
					<li>
						<strong>AI Sağlayıcıları:</strong> Verileri işlemek ve içerik üretmek için (genellikle veriler
						mümkün olduğunca anonimleştirilir).
					</li>
					<li>
						<strong>Analitik Sağlayıcıları:</strong> Uygulamanın nasıl kullanıldığını anlamamıza yardımcı
						olmak için.
					</li>
				</ul>
			</li>
			<li>
				<strong>Yasal Gereklilikler:</strong> Kanunen gerekli olduğunda veya haklarımızı korumak için.
			</li>
			<li>
				<strong>Mülkiyet Devirleri:</strong> Bir birleşme, satış veya varlık devri ile bağlantılı olarak.
			</li>
		</ul>

		<h2>6. Veri Güvenliği ve Saklama</h2>
		<p>
			Kişisel bilgilerinizi korumaya yardımcı olmak için idari, teknik ve fiziksel güvenlik
			önlemleri kullanıyoruz.
		</p>
		<ul>
			<li>
				<strong>Güvenlik:</strong> Verilerinizi saklamak için endüstri standardı şifreleme ve güvenli
				altyapı (Supabase) kullanıyoruz.
			</li>
			<li>
				<strong>Saklama:</strong> Kişisel bilgilerinizi yalnızca bu Gizlilik Politikasında belirtilen
				amaçlar için gerekli olduğu sürece veya yasal yükümlülüklere uymak için saklıyoruz.
			</li>
		</ul>

		<h2>7. Haklarınız</h2>
		<p>Konumunuza bağlı olarak aşağıdaki haklara sahip olabilirsiniz:</p>
		<ul>
			<li>
				<strong>Erişim ve Düzeltme:</strong> Profil bilgilerinizi doğrudan uygulama içinden görüntüleyebilir
				ve düzenleyebilirsiniz.
			</li>
			<li>
				<strong>Hesap Silme:</strong> Hesabınızın ve ilişkili verilerin silinmesini doğrudan uygulama
				ayarları üzerinden veya bizimle iletişime geçerek talep edebilirsiniz. Silme talebi üzerine, kişisel
				verilerinizi aktif veritabanlarımızdan kalıcı olarak kaldıracağız.
			</li>
		</ul>

		<h2>8. Çocukların Gizliliği</h2>
		<p>
			Hizmetimiz 13 yaşın (veya bazı yargı bölgelerinde 16) altındaki bireyler için
			tasarlanmamıştır. Çocuklardan bilerek kişisel bilgi toplamıyoruz. Bir çocuktan kişisel bilgi
			topladığımızı fark edersek, bu bilgileri silmek için adımlar atacağız.
		</p>

		<h2>9. Üçüncü Taraf Bağlantılar</h2>
		<p>
			Uygulama üçüncü taraf web sitelerine veya hizmetlerine bağlantılar içerebilir. Bu tür üçüncü
			tarafların gizlilik uygulamalarından veya içeriğinden sorumlu değiliz.
		</p>

		<h2>10. Bu Gizlilik Politikasındaki Değişiklikler</h2>
		<p>
			Gizlilik Politikamızı zaman zaman güncelleyebiliriz. Herhangi bir değişikliği bu sayfada yeni
			Gizlilik Politikasını yayınlayarak ve "Son Güncelleme" tarihini güncelleyerek size
			bildireceğiz.
		</p>

		<h2>11. İletişim</h2>
		<p>
			Bu Gizlilik Politikası hakkında sorularınız veya yorumlarınız varsa, lütfen bizimle iletişime
			geçin:
		</p>
		<p>
			<strong>E-posta:</strong> support@aisyfit.com<br />
			<strong>Şirket:</strong> AISYLABS LLC
		</p>
	{:else}
		<h1>Privacy Policy for AisyFit</h1>
		<p><strong>Last Updated:</strong> January 5, 2026</p>

		<h2>1. Introduction</h2>
		<p>
			Welcome to <strong>AisyFit</strong> ("we," "our," or "us"). We are committed to protecting your
			privacy and ensuring you have a positive experience on our mobile application and services (collectively,
			the "Service").
		</p>
		<p>
			This Privacy Policy explains how we collect, use, disclose, and safeguard your information
			when you use our AI-powered fitness coaching application. Please read this privacy policy
			carefully. If you do not agree with the terms of this privacy policy, please do not access the
			application.
		</p>

		<h2>2. Information We Collect</h2>
		<p>
			We collect information that identifies, relates to, describes, references, is capable of being
			associated with, or could reasonably be linked, directly or indirectly, with you ("Personal
			Information").
		</p>

		<h3>A. Information You Provide to Us</h3>
		<ul>
			<li>
				<strong>Account Registration:</strong> Name, email address, password, and profile image.
			</li>
			<li>
				<strong>Health and Fitness Data:</strong> Gender, age, weight, height, activity level, fitness
				goals, dietary preferences, allergies, injuries, and workout history.
			</li>
			<li>
				<strong>User Content:</strong> Feedback, logs, check-ins, and any photos you upload (e.g., progress
				photos).
			</li>
		</ul>

		<h3>B. Information Collected Automatically</h3>
		<ul>
			<li>
				<strong>Device Information:</strong> Device type, operating system, unique device identifiers
				(e.g., IDFA, Android ID), and IP address.
			</li>
			<li>
				<strong>Usage Data:</strong> Details of your visits to our application, traffic data, logs, and
				other communication data and the resources that you access and use.
			</li>
			<li>
				<strong>Metrics:</strong> Daily step counts, water intake, and other tracked metrics if functionality
				is enabled and permissions granted.
			</li>
		</ul>

		<h3>C. AI Processing</h3>
		<ul>
			<li>
				We use Artificial Intelligence (AI) to generate personalized workout and diet plans. The
				data you provide (goals, injuries, preferences) is processed by our AI algorithms to create
				these plans.
			</li>
		</ul>

		<h2>3. How We Use Your Information</h2>
		<p>We use the information we collect for the following purposes:</p>
		<ul>
			<li>
				<strong>Provide and Manage the Service:</strong> To create personalized account profiles, generate
				AI-driven workout and diet plans, and track your progress.
			</li>
			<li>
				<strong>Improve the Service:</strong> To analyze usage patterns, train our AI models (on anonymized/aggregated
				data), and fix bugs.
			</li>
			<li>
				<strong>Communication:</strong> To send you updates, security alerts, and support messages.
			</li>
			<li>
				<strong>Compliance:</strong> To comply with legal obligations and enforce our Terms of Use.
			</li>
		</ul>

		<h2>4. Specific Provisions for Health Data</h2>
		<p><strong>AisyFit</strong> treats your health and fitness data with high sensitivity.</p>
		<ul>
			<li>We do <strong>not</strong> sell your personal health data to third parties.</li>
			<li>
				We use your health data solely to provide the fitness and nutrition coaching features of the
				app.
			</li>
			<li>
				If you integrate with Apple HealthKit or Google Fit, we use that data only to update your
				progress within the app and do not use it for advertising purposes.
			</li>
		</ul>

		<h2>5. Sharing Your Information</h2>
		<p>We may share information with:</p>
		<ul>
			<li>
				<strong>Service Providers:</strong> Third-party vendors who perform services for us, such
				as:
				<ul>
					<li><strong>Supabase:</strong> For secure database hosting and authentication.</li>
					<li>
						<strong>AI Providers:</strong> To process data and generate content (though data is typically
						anonymized where possible).
					</li>
					<li>
						<strong>Analytics Providers:</strong> To help us understand how the app is used.
					</li>
				</ul>
			</li>
			<li>
				<strong>Legal Requirements:</strong> If required by law or to protect our rights.
			</li>
			<li>
				<strong>Business Transfers:</strong> In connection with a merger, sale, or asset transfer.
			</li>
		</ul>

		<h2>6. Data Security and Retention</h2>
		<p>
			We use administrative, technical, and physical security measures to help protect your personal
			information.
		</p>
		<ul>
			<li>
				<strong>Security:</strong> We utilize industry-standard encryption and secure infrastructure (Supabase)
				to store your data.
			</li>
			<li>
				<strong>Retention:</strong> We retain your personal information only for as long as is necessary
				for the purposes set out in this Privacy Policy, or to comply with legal obligations.
			</li>
		</ul>

		<h2>7. Your Rights</h2>
		<p>Depending on your location, you may have the following rights:</p>
		<ul>
			<li>
				<strong>Access and Correction:</strong> You can access and edit your profile information directly
				within the app.
			</li>
			<li>
				<strong>Account Deletion:</strong> You can request the deletion of your account and associated
				data directly through the application settings or by contacting us. Upon deletion request, we
				will permanently remove your personal data from our active databases.
			</li>
		</ul>

		<h2>8. Children's Privacy</h2>
		<p>
			Our Service is not intended for individuals under the age of 13 (or 16 in certain
			jurisdictions). We do not knowingly collect personal information from children. If we become
			aware that we have collected personal information from a child, we will take steps to delete
			such information.
		</p>

		<h2>9. Third-Party Links</h2>
		<p>
			The Application may contain links to third-party websites or services. We are not responsible
			for the privacy practices or content of such third parties.
		</p>

		<h2>10. Changes to This Privacy Policy</h2>
		<p>
			We may update our Privacy Policy from time to time. We will notify you of any changes by
			posting the new Privacy Policy on this page and updating the "Last Updated" date.
		</p>

		<h2>11. Contact Us</h2>
		<p>If you have questions or comments about this Privacy Policy, please contact us at:</p>
		<p>
			<strong>Email:</strong> support@aisyfit.com<br />
			<strong>Company:</strong> AISYLABS LLC
		</p>
	{/if}
</div>
