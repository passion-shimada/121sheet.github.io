<!DOCTYPE html>
<html lang="ja">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Complete Introduction Form</title>
    <!-- Tailwind CSS の CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- 印刷時のスタイル（プレビュー部分だけ印刷する） -->
    <style>
      @media print {
        body * {
          visibility: hidden;
        }
        .printable,
        .printable * {
          visibility: visible;
        }
        .printable {
          position: absolute;
          left: 0;
          top: 0;
          width: 100%;
        }
        /* 印刷時に不要な要素は非表示 */
        .no-print {
          display: none;
        }
      }
    </style>
    <!-- React & ReactDOM の UMD ビルド（React 18） -->
    <script crossorigin src="https://unpkg.com/react@18/umd/react.development.js"></script>
    <script crossorigin src="https://unpkg.com/react-dom@18/umd/react-dom.development.js"></script>
    <!-- Babel (JSX のトランスパイル用) -->
    <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
  </head>
  <body class="bg-gray-100">
    <div id="root"></div>
    <script type="text/babel">
      const { useState, useRef, memo } = React;

      // lucide-react の Camera アイコンの代替として SVG を返すコンポーネント
      const Camera = (props) => (
        <svg
          {...props}
          viewBox="0 0 24 24"
          fill="none"
          stroke="currentColor"
          strokeWidth="2"
          strokeLinecap="round"
          strokeLinejoin="round"
        >
          <path d="M23 19a2 2 0 0 1-2 2H3a2 2 0 0 1-2-2V7a2 2 0 0 1 2-2h4l2-3h6l2 3h4a2 2 0 0 1 2 2z" />
          <circle cx="12" cy="13" r="4" />
        </svg>
      );

      // 入力コンポーネントを React.memo でメモ化
      const InputField = memo(function InputField({ label, name, type = "text", value, onChange }) {
        return (
          <div className="mb-4">
            <label className="block text-sm font-bold text-blue-600 mb-1">
              {label}
            </label>
            {type === "textarea" ? (
              <textarea
                name={name}
                value={value}
                onChange={onChange}
                className="w-full p-2 border rounded"
                rows="3"
              />
            ) : (
              <input
                type="text"
                name={name}
                value={value}
                onChange={onChange}
                className="w-full p-2 border rounded"
              />
            )}
          </div>
        );
      });

      const CompleteIntroductionForm = () => {
        const fileInputRef = useRef(null);
        // 「age」キーを追加
        const [formData, setFormData] = useState({
          photoUrl: '',
          name: '',
          age: '',
          nameRomaji: '',
          location: '',
          residence: '',
          residenceYears: '',
          hometown: '',
          specialty: '',
          company: '',
          experience: '',
          careerHistory: '',
          family: '',
          spouse: '',
          pets: '',
          hobbies: '',
          privateInterests: '',  // プライベート情報の「その他の関心ごと」
          secret: '',
          desire: '',
          successKey: '',
          goals: '',
          accomplishments: '',
          networkings: '',
          skills: '',
          gainsInterests: ''     // G.A.I.N.S. の「Interests（興味）」
        });

        const [showPreview, setShowPreview] = useState(false);

        const handleInputChange = (e) => {
          const { name, value } = e.target;
          setFormData((prev) => ({
            ...prev,
            [name]: value
          }));
        };

        const handlePhotoClick = () => {
          fileInputRef.current && fileInputRef.current.click();
        };

        const handlePhotoChange = (e) => {
          const file = e.target.files && e.target.files[0];
          if (file) {
            const reader = new FileReader();
            reader.onloadend = () => {
              setFormData((prev) => ({
                ...prev,
                photoUrl: reader.result
              }));
            };
            reader.readAsDataURL(file);
          }
        };

        // プレビュー表示時にPDF（印刷）を呼び出す
        const handlePrint = () => {
          window.print();
        };

        const PhotoUpload = () => (
          <div className="mb-6">
            <label className="block text-sm font-bold text-blue-600 mb-2">
              顔写真
            </label>
            <div className="flex items-center space-x-4">
              {formData.photoUrl ? (
                <img
                  src={formData.photoUrl}
                  alt="プロフィール写真"
                  className="w-32 h-32 object-cover rounded"
                />
              ) : (
                <div className="w-32 h-32 bg-gray-100 flex items-center justify-center rounded">
                  <Camera className="w-8 h-8 text-gray-400" />
                </div>
              )}
              <input
                type="file"
                ref={fileInputRef}
                onChange={handlePhotoChange}
                accept="image/*"
                className="hidden"
              />
              <button
                type="button"
                onClick={handlePhotoClick}
                className="px-4 py-2 bg-gray-100 text-blue-600 rounded hover:bg-gray-200"
              >
                写真を選択
              </button>
            </div>
          </div>
        );

        const PreviewSection = ({ title, data }) => (
          <div className="mb-6">
            <h3 className="text-lg font-bold mb-2">
              {title}
            </h3>
            <div className="bg-gray-50 p-4 rounded">
              {Object.entries(data).map(([key, value]) => (
                <div key={key} className="mb-2">
                  <span className="font-bold text-blue-600">{key}:</span> {value}
                </div>
              ))}
            </div>
          </div>
        );

        if (showPreview) {
          return (
            <div className="max-w-4xl mx-auto p-6 bg-white printable">
              <div className="flex flex-col sm:flex-row sm:justify-between items-start sm:items-center mb-6 no-print">
                <div className="flex items-center space-x-6">
                  {formData.photoUrl && (
                    <img
                      src={formData.photoUrl}
                      alt="プロフィール写真"
                      className="w-32 h-32 object-cover rounded"
                    />
                  )}
                  <div>
                    <h2 className="text-2xl font-bold">
                      {formData.name}
                      {formData.age && (
                        <span className="ml-2 text-xl">{formData.age}歳</span>
                      )}
                    </h2>
                    <p className="text-xl text-blue-600">{formData.nameRomaji}</p>
                  </div>
                </div>
                <div className="mt-4 sm:mt-0 space-x-2">
                  <button
                    onClick={handlePrint}
                    className="px-6 py-2 bg-green-500 text-white rounded hover:bg-green-600"
                  >
                    PDFで出力
                  </button>
                  <button
                    onClick={() => setShowPreview(false)}
                    className="px-6 py-2 bg-blue-500 text-white rounded hover:bg-blue-600"
                  >
                    編集に戻る
                  </button>
                </div>
              </div>

              <PreviewSection
                title={
                  <>
                    <span className="text-3xl mr-2">🏢</span>
                    【基本情報・職歴・キャリア】
                  </>
                }
                data={{
                  "所在地": formData.location,
                  "居住地": formData.residence,
                  "居住年数": formData.residenceYears,
                  "出身地": formData.hometown,
                  "専門分野": formData.specialty,
                  "会社名": formData.company,
                  "経験年数": formData.experience,
                  "職歴": formData.careerHistory
                }}
              />

              <PreviewSection
                title={
                  <>
                    <span className="text-3xl mr-2">🏡</span>
                    【プライベート情報】
                  </>
                }
                data={{
                  "家族": formData.family,
                  "配偶者": formData.spouse,
                  "ペット": formData.pets,
                  "趣味": formData.hobbies,
                  "その他の関心ごと": formData.privateInterests
                }}
              />

              <PreviewSection
                title={
                  <>
                    <span className="text-3xl mr-2">⭐</span>
                    【自己PR・価値観】
                  </>
                }
                data={{
                  "誰も知らない私": formData.secret,
                  "私の強い願望": formData.desire,
                  "私の成功の鍵": formData.successKey
                }}
              />

              <PreviewSection
                title={
                  <>
                    <span className="text-3xl mr-2">🎯</span>
                    【G.A.I.N.S.】
                  </>
                }
                data={{
                  "Goals（目標）": formData.goals,
                  "Accomplishment（実績）": formData.accomplishments,
                  "Interests（興味）": formData.gainsInterests,
                  "Networks（人脈）": formData.networkings,
                  "Skills（スキル）": formData.skills
                }}
              />
            </div>
          );
        }

        return (
          <div className="max-w-4xl mx-auto p-6">
            {/* フォーム送信によるリロード防止 */}
            <form className="space-y-8" onSubmit={(e) => e.preventDefault()}>
              <PhotoUpload />

              {/* 基本情報・職歴・キャリア セクション */}
              <div>
                <h2 className="text-xl font-bold mb-4">
                  <span className="text-3xl mr-2">🏢</span>
                  【基本情報・職歴・キャリア】
                </h2>
                {/* 氏名と年齢を横並びに表示 */}
                <div className="flex gap-4">
                  <div className="flex-1">
                    <InputField label="氏名" name="name" value={formData.name} onChange={handleInputChange} />
                  </div>
                  <div className="w-24">
                    <label className="block text-sm font-bold text-blue-600 mb-1">年齢</label>
                    <div className="flex items-center border rounded p-2">
                      <input
                        type="text"
                        name="age"
                        value={formData.age}
                        onChange={handleInputChange}
                        className="w-full outline-none"
                      />
                      <span className="ml-1">歳</span>
                    </div>
                  </div>
                </div>
                <InputField label="氏名（ローマ字）" name="nameRomaji" value={formData.nameRomaji} onChange={handleInputChange} />
                <InputField label="所在地" name="location" value={formData.location} onChange={handleInputChange} />
                <InputField label="居住地" name="residence" value={formData.residence} onChange={handleInputChange} />
                <InputField label="居住年数" name="residenceYears" value={formData.residenceYears} onChange={handleInputChange} />
                <InputField label="出身地" name="hometown" value={formData.hometown} onChange={handleInputChange} />
                <InputField label="専門分野" name="specialty" value={formData.specialty} onChange={handleInputChange} />
                <InputField label="会社名" name="company" value={formData.company} onChange={handleInputChange} />
                <InputField label="経験年数" name="experience" value={formData.experience} onChange={handleInputChange} />
                <InputField label="職歴" name="careerHistory" type="textarea" value={formData.careerHistory} onChange={handleInputChange} />
              </div>

              {/* プライベート情報 セクション */}
              <div>
                <h2 className="text-xl font-bold mb-4">
                  <span className="text-3xl mr-2">🏡</span>
                  【プライベート情報】
                </h2>
                <InputField label="家族" name="family" value={formData.family} onChange={handleInputChange} />
                <InputField label="配偶者" name="spouse" value={formData.spouse} onChange={handleInputChange} />
                <InputField label="ペット" name="pets" value={formData.pets} onChange={handleInputChange} />
                <InputField label="趣味" name="hobbies" value={formData.hobbies} onChange={handleInputChange} />
                <InputField label="その他の関心ごと" name="privateInterests" value={formData.privateInterests} onChange={handleInputChange} />
              </div>

              {/* 自己PR・価値観 セクション */}
              <div>
                <h2 className="text-xl font-bold mb-4">
                  <span className="text-3xl mr-2">⭐</span>
                  【自己PR・価値観】
                </h2>
                <InputField label="誰も知らない私" name="secret" type="textarea" value={formData.secret} onChange={handleInputChange} />
                <InputField label="私の強い願望" name="desire" type="textarea" value={formData.desire} onChange={handleInputChange} />
                <InputField label="私の成功の鍵" name="successKey" type="textarea" value={formData.successKey} onChange={handleInputChange} />
              </div>

              {/* G.A.I.N.S. セクション */}
              <div>
                <h2 className="text-xl font-bold mb-4">
                  <span className="text-3xl mr-2">🎯</span>
                  【G.A.I.N.S.】
                </h2>
                <InputField label="Goals（目標）" name="goals" type="textarea" value={formData.goals} onChange={handleInputChange} />
                <InputField label="Accomplishment（実績）" name="accomplishments" type="textarea" value={formData.accomplishments} onChange={handleInputChange} />
                <InputField label="Interests（興味）" name="gainsInterests" type="textarea" value={formData.gainsInterests} onChange={handleInputChange} />
                <InputField label="Networks（人脈）" name="networkings" type="textarea" value={formData.networkings} onChange={handleInputChange} />
                <InputField label="Skills（スキル）" name="skills" type="textarea" value={formData.skills} onChange={handleInputChange} />
              </div>

              <button
                type="button"
                onClick={() => setShowPreview(true)}
                className="w-full px-6 py-2 bg-blue-500 text-white rounded hover:bg-blue-600"
              >
                プレビューを表示
              </button>
            </form>
          </div>
        );
      };

      ReactDOM.createRoot(document.getElementById('root')).render(<CompleteIntroductionForm />);
    </script>
  </body>
</html>
