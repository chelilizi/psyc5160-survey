PSYC5160 Survey v3

Participant-facing flow:
Nickname + Code -> Consent/background -> Demographics -> One-time audio -> 8 MC -> 7 ratings -> Submit

Participants never see or select a version. The Code selects the internal survey_version and MP3:

Participant code | survey_version | filename   | internal description
HK314            | 1              | audio1.mp3 | Godfrey’s friend_Original
LM527            | 2              | audio2.mp3 | Godfrey's friend_1.3x
NP683            | 3              | audio3.mp3 | Klowie 1st friend_Original
QR246            | 4              | audio4.mp3 | Klowie 1st friend_1.3x
ST915            | 5              | audio5.mp3 | Klowie 2nd friend_Original
VX408            | 6              | audio6.mp3 | Klowie 2nd friend_1.3x

Before deployment:
1. Run supabase_update_v3.sql once in Supabase SQL Editor.
2. Open index.html and replace YOUR_SUPABASE_URL and YOUR_SUPABASE_ANON_KEY with your own Project URL and publishable key.
3. Keep index.html and audio1.mp3 ... audio6.mp3 in the same folder.
4. Replace each test MP3 with the final MP3 using exactly the same filename.
5. Redeploy the whole folder to the SAME Netlify site to keep the production URL.

If you later change any Code in index.html, also change the same Code in supabase_update_v3.sql / database constraints and RLS policy.
