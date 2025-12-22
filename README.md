# Sistem-Pakar




def tanya(gejala):
    return input(f"Apakah Anda mengalami {gejala}? (y/n): ").lower() == "y"

def sistem_pakar():
    print("=== SISTEM PAKAR DIAGNOSIS PENYAKIT RINGAN MUSIM HUJAN ===\n")

    demam = tanya("demam")
    batuk = tanya("batuk")
    pilek = tanya("pilek")
    bersin = tanya("bersin")
    nyeri_otot = tanya("nyeri otot")
    sakit_kepala = tanya("sakit kepala")
    tenggorokan_sakit = tanya("sakit tenggorokan")
    nyeri_menelan = tanya("nyeri saat menelan")
    suara_serak = tanya("suara serak")
    mual = tanya("mual")
    perut_kembung = tanya("perut kembung")
    diare = tanya("diare")
    lemas = tanya("lemas")
    mata_gatal = tanya("mata gatal")
    hidung_gatal = tanya("hidung gatal")
    sesak = tanya("sesak napas ringan")

    print("\n=== HASIL DIAGNOSIS ===")

    if demam and batuk and nyeri_otot:
        print("Diagnosis : Influenza")
        print("Rekomendasi : Paracetamol, Vitamin C, Istirahat cukup")

    elif pilek and bersin and not demam:
        print("Diagnosis : Common Cold (Pilek)")
        print("Rekomendasi : Obat flu ringan, minum air hangat")

    elif demam and sakit_kepala and lemas:
        print("Diagnosis : Demam")
        print("Rekomendasi : Paracetamol, perbanyak cairan")

    elif batuk and tenggorokan_sakit:
        print("Diagnosis : Batuk")
        print("Rekomendasi : Obat batuk, madu, istirahat")

    elif tenggorokan_sakit and nyeri_menelan and suara_serak:
        print("Diagnosis : Sakit Tenggorokan")
        print("Rekomendasi : Lozenges, air hangat")

    elif perut_kembung and mual:
        print("Diagnosis : Masuk Angin")
        print("Rekomendasi : Obat herbal masuk angin, istirahat")

    elif diare and mual and lemas:
        print("Diagnosis : Diare Ringan")
        print("Rekomendasi : Oralit, zinc")

    elif sakit_kepala and not demam:
        print("Diagnosis : Sakit Kepala")
        print("Rekomendasi : Paracetamol, istirahat")

    elif bersin and mata_gatal and hidung_gatal:
        print("Diagnosis : Alergi")
        print("Rekomendasi : Antihistamin")

    elif batuk and demam and sesak:
        print("Diagnosis : ISPA Ringan")
        print("Rekomendasi : Obat batuk, antipiretik, konsultasi bila memburuk")

    else:
        print("Diagnosis tidak dapat ditentukan")
        print("Disarankan konsultasi ke tenaga medis")


sistem_pakar()
