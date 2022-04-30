 <div class="par">
              <label for="fechaNacimiento">Fecha de Nacimiento</label>
              <input
                type="date"
                id="fechaNacimiento"
                v-model="fechaNacimiento"
                name="fechaNacimiento"
                :class="{ revisar: revisiones.fechaNacimiento }"
              />
              <div v-if="revisiones.fechaNacimiento">
                <p>
                  <span class="revisar">
                    Por favor completa tu fecha de Nacimiento
                  </span>
                </p>
              </div>
            </div>
            <br /><br />