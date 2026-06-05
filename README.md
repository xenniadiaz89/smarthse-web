import streamlit as st

# Configuración de página (Debe ser la primera línea después de los imports)
st.set_page_config(page_title="Smart HSE Chile", page_icon="🛡️", layout="centered")

# Estilos CSS personalizados para un look profesional
st.markdown("""
    <style>
    .main { background-color: #f5f7f9; }
    .stButton>button { width: 100%; border-radius: 5px; height: 3em; background-color: #004a99; color: white; }
    h1 { color: #004a99; }
    </style>
    """, unsafe_allow_html=True)

# Título y presentación
st.title("🛡️ Smart HSE Chile")
st.subheader("Transformando la Gestión de Seguridad y Salud Ocupacional")

st.markdown("""
Bienvenido a la plataforma centralizada para la automatización de riesgos. 
Esta herramienta permite gestionar matrices MIPER, registros legales y auditorías 
de forma eficiente y trazable.
""")

# Sección de Normas (La que necesitabas)
st.divider()
st.header("📋 Normas y Estándares")
st.info("""
**Nuestra metodología se basa en:**
1. **Cumplimiento Legal:** Seguimiento estricto bajo Ley 16.744 y DS 44.
2. **Estandarización:** Procesos unificados para contratistas mineros.
3. **Trazabilidad:** Registro automatizado de cada tarea y control de riesgos.
""")

# Sección de acciones
st.divider()
st.subheader("¿Cómo podemos ayudar hoy?")
col1, col2 = st.columns(2)

with col1:
    if st.button("Ir a Matriz Legal"):
        st.write("Cargando módulo de leyes...")

with col2:
    if st.button("Gestionar Auditoría"):
        st.write("Iniciando auditoría interna...")

# Footer
st.markdown("---")
st.caption("© 2026 Smart HSE Chile - Soluciones de Marketing Digital y Brandi")
