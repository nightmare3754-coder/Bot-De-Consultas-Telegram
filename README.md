<?xml version="1.0" encoding="UTF-8"?>
<bot>
    <metadata>
        <name>Mirai Buscas - Bot de Consultas Telegram</name>
        <version>1.0.0</version>
        <description>Plataforma de consultas mais completa e ágil do mercado</description>
        <last_update>2025-10-24</last_update>
    </metadata>

    <!-- PERFIL DO USUÁRIO -->
    <user_profile>
        <id>6370311807</id>
        <status>Ativo</status>
        <current_plan>Plano Premium 90 dias</current_plan>
        <affiliate_balance>R$ 0.00</affiliate_balance>
        <message>Seja bem-vindo(a) à plataforma de consultas mais completa e ágil do mercado!</message>
    </user_profile>

    <!-- FUNCIONALIDADES PRINCIPAIS -->
    <features>
        <feature>
            <title>Consultar dados completos</title>
            <description>CPF, RG, CEP, Placa, etc.</description>
            <icon>📊</icon>
        </feature>
        <feature>
            <title>Adquirir planos de uso ilimitado</title>
            <description>Acesso completo a todas as bases</description>
            <icon>💳</icon>
        </feature>
        <feature>
            <title>Acompanhar ganhos e planos ativos</title>
            <description>Gerenciamento de conta e histórico</description>
            <icon>📈</icon>
        </feature>
    </features>

    <!-- MÓDULOS DE CONSULTA -->
    <consultation_modules>
        <category name="Documentos Oficiais">
            <module id="cpf" name="CPF" />
            <module id="cnpj" name="CNPJ" />
            <module id="rg" name="RG" />
            <module id="cep" name="CEP" />
            <module id="cnh" name="CNH" />
            <module id="serasa" name="Serasa" />
        </category>

        <category name="Dados Pessoais">
            <module id="nomefull" name="Nome Completo" />
            <module id="email" name="Email" />
            <module id="telefone" name="Telefone" />
            <module id="nometim" name="Nome Tim" />
        </category>

        <category name="Informações Veiculares">
            <module id="placa" name="Placa" />
            <module id="renavam" name="Renavam" />
            <module id="motor" name="Motor" />
            <module id="chassi" name="Chassi" />
        </category>

        <category name="Tributários e Fiscais">
            <module id="cpf_receita" name="CPF Receita" />
            <module id="renda" name="Renda" />
            <module id="processes" name="Processos" />
            <module id="cpfsus" name="CPF Suspenso" />
        </category>

        <category name="Informações Adicionais">
            <module id="nomejbr" name="Nome JBR" />
            <module id="emailfull" name="Email Full" />
            <module id="score" name="Score" />
        </category>
    </consultation_modules>

    <!-- MÓDULOS DE FOTO -->
    <photo_modules>
        <title>Escolha o módulo de foto desejado</title>
        <button>
            <id>foto_ro</id>
            <label>FOTO RO</label>
            <state>default</state>
        </button>
        <button>
            <id>foto_ce</id>
            <label>FOTO CE</label>
            <state>default</state>
        </button>
        <button>
            <id>foto_sp</id>
            <label>FOTO SP</label>
            <state>default</state>
        </button>
        <button>
            <id>foto_ma</id>
            <label>FOTO MA</label>
            <state>default</state>
        </button>
        <button>
            <id>foto_rj</id>
            <label>FOTO RJ</label>
            <state>default</state>
        </button>
        <button>
            <id>voltar</id>
            <label>VOLTAR</label>
            <type>back</type>
            <icon>↩️</icon>
        </button>
    </photo_modules>

    <!-- OPÇÕES DE CONSULTA -->
    <query_options>
        <title>Escolha uma das opções de consulta disponíveis abaixo</title>
        <option_grid>
            <row>
                <button id="score" label="SCORE" />
                <button id="cpf_receita" label="CPF RECEITA" />
            </row>
            <row>
                <button id="cep" label="CEP" />
                <button id="renda" label="RENDA" />
            </row>
            <row>
                <button id="cnpj" label="CNPJ" />
                <button id="processes" label="PROCESSOS" />
            </row>
            <row>
                <button id="serasa" label="SERASA" />
                <button id="nomejbr" label="NOMEJBR" />
            </row>
            <row>
                <button id="emailfull" label="EMAILFULL" />
                <button id="rg" label="RG" />
            </row>
            <row>
                <button id="cpfsus" label="CPFSUS" />
                <button id="cpf" label="CPF" />
            </row>
            <row>
                <button id="nomefull" label="NOMEFULL" />
                <button id="telefone" label="TELEFONE" />
            </row>
            <row>
                <button id="placa" label="PLACA" />
                <button id="motor" label="MOTOR" />
            </row>
            <row>
                <button id="renavam" label="RENAVAM" />
                <button id="nome" label="NOME" />
            </row>
            <row>
                <button id="pis" label="PIS" />
                <button id="cpf_full" label="CPF FULL" />
            </row>
            <row>
                <button id="cepfull" label="CEPFULL" />
                <button id="email" label="EMAIL" />
            </row>
            <row>
                <button id="nometim" label="NOMETIM" />
                <button id="chassi" label="CHASSI" />
            </row>
        </option_grid>
        <button>
            <id>modulos_foto</id>
            <label>MÓDULOS DE FOTO</label>
            <icon>📸</icon>
        </button>
        <button>
            <id>voltar</id>
            <label>VOLTAR</label>
            <type>back</type>
            <icon>↩️</icon>
        </button>
    </query_options>

    <!-- MENU PRINCIPAL -->
    <main_menu>
        <button>
            <id>consultas</id>
            <label>Consultas</label>
            <icon>🔍</icon>
            <action>show_consultation_modules</action>
        </button>
        <button>
            <id>comprar_planos</id>
            <label>Comprar Planos</label>
            <icon>💳</icon>
            <action>show_plans</action>
        </button>
        <button>
            <id>meus_planos</id>
            <label>Meus Planos</label>
            <icon>📋</icon>
            <action>show_active_plans</action>
        </button>
        <button>
            <id>suporte</id>
            <label>Suporte</label>
            <icon>💬</icon>
            <action>open_support</action>
        </button>
        <button>
            <id>perfil</id>
            <label>Perfil</label>
            <icon>👤</icon>
            <action>show_profile</action>
        </button>
    </main_menu>

    <!-- PLANOS DISPONÍVEIS -->
    <plans>
        <plan>
            <name>Plano Premium 90 dias</name>
            <duration>90 dias</duration>
            <price>Consultável</price>
            <features>
                <feature>Consultas ilimitadas</feature>
                <feature>Acesso a todas as bases</feature>
                <feature>Suporte prioritário</feature>
                <feature>Atualizações em tempo real</feature>
                <feature>Histórico de consultas completo</feature>
                <feature>Sem limite de requisições</feature>
            </features>
            <status>Ativo</status>
        </plan>
    </plans>

    <!-- TERMOS DE SERVIÇO -->
    <terms_of_service>
        <last_update>2025-10-24</last_update>
        <content>
            <term>Respeito aos direitos autorais e privacidade</term>
            <term>Cancelamento de plano em casos de abuso</term>
            <term>Proteção contra bugs, erros e violações de diretrizes</term>
            <term>Conformidade com legislação aplicável (LGPD)</term>
            <term>Direito de cancelar plano em caso de abuso de bugs, erros ou violação de diretrizes</term>
        </content>
    </terms_of_service>

    <!-- SEGURANÇA -->
    <security>
        <feature>Encriptação de dados em trânsito</feature>
        <feature>Conformidade com LGPD</feature>
        <feature>Acesso seguro via autenticação Telegram</feature>
        <feature>Auditoria regular de sistemas</feature>
        <feature>Proteção de dados pessoais</feature>
    </security>

    <!-- CONTATO E SUPORTE -->
    <support>
        <channel type="telegram">
            <name>Telegram Direct</name>
            <description>Acesse via bot para suporte rápido</description>
        </channel>
        <channel type="email">
            <name>Email</name>
            <description>Disponível na seção de Suporte</description>
        </channel>
        <channel type="priority">
            <name>Atendimento Prioritário</name>
            <description>Incluso em planos Premium</description>
        </channel>
    </support>

    <!-- INFORMAÇÕES ADICIONAIS -->
    <additional_info>
        <reading_speed>LEITURA RÁPIDA</reading_speed>
        <last_message_time>23:34</last_message_time>
        <developer_message>Desenvolvido com ❤️ para facilitar sua vida</developer_message>
    </additional_info>
</bot>
